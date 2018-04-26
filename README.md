h


Process = csgo.exe
DllName = client.dll
msgbox, WAIT WAIT WAIT

Process, Exist, %Process%
PID = %ErrorLevel%
SetFormat, Integer, Hex
Base := GetDllBase(DllName, PID)

start:=0x00000000
loop {
start:=start+0x1000
check:=ReadMemory(start+0x4,"Counter-Strike: Global Offensive")
check2:=ReadMemory(check,"Counter-Strike: Global Offensive")

if (check2==0x6574616D)


{

break
}
if (start>0xDDDDDDDD)
{
msgbox, Something went wrong O.o
}

}
offset:=start+0x550
end:=start+0x2000

loop
{
offset:=offset+0x4
check:=ReadMemory(offset,"Counter-Strike: Global Offensive")
checka:=check+0x1c
check2:=ReadMemory(check+0x1c,"Counter-Strike: Global Offensive")
if (check2==0x72617065)
{
break
}
if (offset>end)
{
msgbox, something went wrong OMG
}
}

msgbox, OMG!WALLHACKER!!! D:

offsets3:=offset

t1:=ReadMemory(offsets3,"Counter-Strike: Global Offensive")
t2:=ReadMemory(offsets3+0x8,"Counter-Strike: Global Offensive")
t3:=ReadMemory(offsets3+0x10,"Counter-Strike: Global Offensive")
t4:=ReadMemory(offsets3+0x18,"Counter-Strike: Global Offensive")
t5:=ReadMemory(offsets3+0x20,"Counter-Strike: Global Offensive")
t6:=ReadMemory(offsets3+0x28,"Counter-Strike: Global Offensive")
t7:=ReadMemory(offsets3+0x30,"Counter-Strike: Global Offensive")

offsetsct:=offsets3+0x30+0xC0

ct1:=ReadMemory(offsetsct,"Counter-Strike: Global Offensive")
ct2:=ReadMemory(offsetsct+0x8,"Counter-Strike: Global Offensive")
ct3:=ReadMemory(offsetsct+0x10,"Counter-Strike: Global Offensive")
ct4:=ReadMemory(offsetsct+0x18,"Counter-Strike: Global Offensive")
ct5:=ReadMemory(offsetsct+0x20,"Counter-Strike: Global Offensive")
ct6:=ReadMemory(offsetsct+0x28,"Counter-Strike: Global Offensive")
ct7:=ReadMemory(offsetsct+0x638,"Counter-Strike: Global Offensive")


t11:=t1+0x96D
t111:=ReadMemoryString(t11,"Counter-Strike: Global Offensive")
rewritetex(t111,t11)
t22:=t2+0xC0F
t222:=ReadMemoryString(t22,"Counter-Strike: Global Offensive")
rewritetex(t222,t22)
t33:=t3+0x45D
t333:=ReadMemoryString(t33,"Counter-Strike: Global Offensive")
rewritetex(t333,t33)
t44:=t4+0x7e1
t444:=ReadMemoryString(t44,"Counter-Strike: Global Offensive")
rewritetex(t444,t44)
t55:=t5+0xACC
t555:=ReadMemoryString(t55,"Counter-Strike: Global Offensive")
rewritetex(t555,t55)
t66:=t6+0xFD
t666:=ReadMemoryString(t66,"Counter-Strike: Global Offensive")
rewritetex(t666,t66)
t77:=t7+0x838
t777:=ReadMemoryString(t77,"Counter-Strike: Global Offensive")
rewritetex(t777,t77)



ct11:=ct1+0x27D
ct111:=ReadMemoryString(ct11,"Counter-Strike: Global Offensive")
rewritetex2(ct111,ct11)
ct22:=ct2+0x219d
t222:=ReadMemoryString(ct22,"Counter-Strike: Global Offensive")
rewritetex2(ct222,ct22)
ct33:=ct3+0x378
ct333:=ReadMemoryString(ct33,"Counter-Strike: Global Offensive")
rewritetex2(ct333,ct33)
ct44:=ct4+0x7e1
ct444:=ReadMemoryString(ct44,"Counter-Strike: Global Offensive")
rewritetex2(ct444,ct44)
ct55:=ct5+0xA70
ct555:=ReadMemoryString(ct55,"Counter-Strike: Global Offensive")
rewritetex2(ct111,ct11)
ct66:=ct6+0x111
ct666:=ReadMemoryString(ct66,"Counter-Strike: Global Offensive")
rewritetex2(ct666,ct66)
ct77:=ct7+0xEB7
ct777:=ReadMemoryString(ct77,"Counter-Strike: Global Offensive")
rewritetex2(ct777,ct77)








ExitApp


rewritetex(Haystack,offsettex)
{

Needle = "$rimlight"
StringGetPos, pos, Haystack, %Needle%
if (pos >= 0)
{ WriteMemory(0x6E676924,offsettex+pos+0x0,"Counter-Strike: Global Offensive")
WriteMemory(0x7A65726F,offsettex+pos+0x4,"Counter-Strike: Global Offensive")
WriteMemory(0x20203120,offsettex+pos+0x8,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0xC,"Counter-Strike: Global Offensive")
WriteMemory(0x6C6F6324,offsettex+pos+0x10,"Counter-Strike: Global Offensive")
WriteMemory(0x2220726F,offsettex+pos+0x14,"Counter-Strike: Global Offensive")
WriteMemory(0x3020395B,offsettex+pos+0x18,"Counter-Strike: Global Offensive")
WriteMemory(0x225D3020,offsettex+pos+0x1C,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0x20,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0x24,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0x28,"Counter-Strike: Global Offensive")
}
}

rewritetex2(Haystack,offsettex)
{

Needle = "$rimlight"
StringGetPos, pos, Haystack, %Needle%
if (pos >= 0)
{ WriteMemory(0x6E676924,offsettex+pos+0x0,"Counter-Strike: Global Offensive")
WriteMemory(0x7A65726F,offsettex+pos+0x4,"Counter-Strike: Global Offensive")
WriteMemory(0x20203120,offsettex+pos+0x8,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0xC,"Counter-Strike: Global Offensive")
WriteMemory(0x6C6F6324,offsettex+pos+0x10,"Counter-Strike: Global Offensive")
WriteMemory(0x2220726F,offsettex+pos+0x14,"Counter-Strike: Global Offensive")
WriteMemory(0x3020305B,offsettex+pos+0x18,"Counter-Strike: Global Offensive")
WriteMemory(0x225D3920,offsettex+pos+0x1C,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0x20,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0x24,"Counter-Strike: Global Offensive")
WriteMemory(0x0A0D0A0D,offsettex+pos+0x28,"Counter-Strike: Global Offensive")
}
}





ReadMemory(MADDRESS,PROGRAM)
{
winget, pid, PID, %PROGRAM%
VarSetCapacity(MVALUE,4,0)
ProcessHandle := DllCall("OpenProcess", "Int", 24, "Char", 0, "UInt", pid, "UInt")
DllCall("ReadProcessMemory","UInt",ProcessHandle,"UInt",MADDRESS,"Str",MVALUE,"UInt",4,"UInt *",0)
Loop 4
result += *(&MVALUE + A_Index-1) << 8*(A_Index-1)
return, result
}






WriteMemory(WVALUE,MADDRESS,PROGRAM)
{
winget, pid, PID, %PROGRAM%



ProcessHandle := DllCall("OpenProcess", "int", 2035711, "char", 0, "UInt", PID, "UInt")
DllCall("WriteProcessMemory", "UInt", ProcessHandle, "UInt", MADDRESS, "Uint*", WVALUE,"Uint", 4, "Uint *", 0)

DllCall("CloseHandle", "int", ProcessHandle)
return
}



GetDllBase(DllName, PID = 0)
{
TH32CS_SNAPMODULE := 0x00000008
INVALID_HANDLE_VALUE = -1
VarSetCapacity(me32, 548, 0)
NumPut(548, me32)
snapMod := DllCall("CreateToolhelp32Snapshot", "Uint", TH32CS_SNAPMODULE
, "Uint", PID)
If (snapMod = INVALID_HANDLE_VALUE) {
Return 0
}
If (DllCall("Module32First", "Uint", snapMod, "Uint", &me32)){
while(DllCall("Module32Next", "Uint", snapMod, "UInt", &me32)) {
If !DllCall("lstrcmpi", "Str", DllName, "UInt", &me32 + 32) {
DllCall("CloseHandle", "UInt", snapMod)
Return NumGet(&me32 + 20)
}
}
}
DllCall("CloseHandle", "Uint", snapMod)
Return 0
}


ReadMemoryString(MADDRESS,PROGRAM)
{
winget, pid, PID, %PROGRAM%

ProcessHandle := DllCall("OpenProcess", "Int", 24, "Char", 0, "UInt", pid, "Uint")
teststr =
Loop 32
{
Output := "x"
tempVar := DllCall("ReadProcessMemory", "UInt", ProcessHandle, "UInt", MADDRESS, "str", Output, "Uint", 1, "Uint *", 0)
if (ErrorLevel or !tempVar)
{
DllCall("CloseHandle", "int", ProcessHandle)
return teststr
}



teststr = %teststr%%Output%
MADDRESS++
}
DllCall("CloseHandle", "int", ProcessHandle)
return, teststr

}
