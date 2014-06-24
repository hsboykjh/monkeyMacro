monkeyMacro
===========

Monkey Macro Tool for Android Apps


CTCAE TEST Macro 

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


run
adb shell monkey -f scriptFile count(number)
( ex: adb shell monkey -f testscript.txt 10 )
