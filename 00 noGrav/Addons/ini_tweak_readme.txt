
In addition to this plugin, add/replace the following lines in your Skyrim.ini:

[Combat]
f1PArrowTiltUpAngle=0.2
f1PboltTiltUpAngle=0.2
f3PArrowTiltUpAngle=0.7
fMagnetismLookingMult=-0.0
fMagnetismStrafeHeadingMult=-0.0






(Explanation following if you're interested)


What do these settings do?
	Lining up fired arrows/bolts with your crosshair/screen center in 1st & 3rd person:
			f1PArrowTiltUpAngle=0.2
			f1PboltTiltUpAngle=0.2
			f3PArrowTiltUpAngle=0.7
	
	Stop arrows from impacting targets they pass in close proximity:
			fMagnetismLookingMult=-0.0
			fMagnetismStrafeHeadingMult=-0.0
			
		You can use either 0.0 or -0.0 here, but personally I've had more success with -0
			(Detailed explanation below if you're interested)



(Magnetism value explanation)
			
			Normally we would consider -0 to not be valid. However, with computer code this works a little differently.
			Since the first character of the line is 'f', this means the value is a floating-point variable, often called a "float".
			Floating-point variables are capable of holding "real" numbers in both positive and negative. 
			To give you an idea as to why a float can be either a 0 or a -0 consider the following 
			32-bit representations of 2 float values below:
			
					0 00000000 00000000000000000000000
					1 00000000 00000000000000000000000
					^	  ^				  ^
				  sign   exponent	   fraction
				  
			As you can see, the only difference between these values is the first, or "sign" bit. The sign bit is used to determine 
			whether a value is positive or negative, which is why a float can be -0.
			
			I've been playing around with the magnetism ini setting for a while, and based on my testing, 
			a magnetism value of 0 does not appear to actually turn off magnetism entirely. I tried using a negative value here, but it 
			(somewhat obviously) caused arrows to miss, even when they had visibly impacted the target.
			And that's why I tried using -0.0, which on my system, appears to have actually worked! 
			(Likely due to the game engine not expecting -0 to be a possible input, but this doesn't cause any instability.)