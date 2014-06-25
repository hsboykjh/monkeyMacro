
#monkeyMacro
======================


#Monkey Macro Tool for Android Apps


###step
####1. Make scripts on Desktop.
	testTouchScripts.txt
	
	
	speed= 1000
	start data >>
	DispatchPointer(0, 0, 0, 920, 1700, 0,0,0,0,0,0,0)  
	DispatchPointer(0, 0, 1, 920, 1700, 0,0,0,0,0,0,0) 
	UserWait(3000)
	DispatchPress(KEYCODE_HOME)
	UserWait(500)
	DispatchPointer(0, 0, 0, 1000, 480, 0,0,0,0,0,0,0)  
	DispatchPointer(0, 0, 1, 1000, 480, 0,0,0,0,0,0,0) 
	UserWait(4000)
	DispatchPointer(0, 0, 0, 500, 1200, 0,0,0,0,0,0,0)  
	DispatchPointer(0, 0, 1, 500, 1200, 0,0,0,0,0,0,0) 
	UserWait(500)
	DispatchPointer(0, 0, 0, 500, 1200, 0,0,0,0,0,0,0)  
	DispatchPointer(0, 0, 1, 500, 1200, 0,0,0,0,0,0,0) 
	UserWait(500)
	DispatchPress(KEYCODE_BACK)
	UserWait(500)
	DispatchPointer(0, 0, 0, 500, 1200, 0,0,0,0,0,0,0)  
	DispatchPointer(0, 0, 1, 500, 1200, 0,0,0,0,0,0,0) 
	UserWait(2000)
	

####2. Transfer the script files to the android device using adb.
	adb push /path/to/local/file /mnt/sdcard/path/to/file
####3. Run the script file.
	adb shell monkey -f scriptFile count(number)
	( ex: adb shell monkey -f testTouchScripts.txt 10 )
