# RegistrationFreeCOM
Inject DLL Prototype using Microsoft.Windows.ACTCTX COM Object

Extract Files to C:\Tools\regfree

CScript Example:
C:\Windows\syswow64\cscript.exe regfree.js

PowerShell Example:   Be Sure to Use x86 PowwerShell for my POC
$a = New-Object -COM Microsoft.Windows.ActCTX
$a.Manifest = "C:\Tools\regfree\SideBySide.X.manifest"
$a.CreateObject("SideBySide.X")

The DLL can be any dll you create with code in DLL_PROCESS_ATTACH

This may be useful.  I don't know.  I think its interesting.


