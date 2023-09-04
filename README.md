# TeamsImplant
TeamsImplant
TeamsImplant
This project is a stealthy teams implant that proxies the urlmon.dll that teams uses compile and throw this bad boy in the teams directory as urlmon.dll and you got yourself a persistence backdoor whenever teams runs by a user or at startup.

Features:

Mutex so you don't get spammed with 10 shells when teams creates 10 different teams processes and loads the proxy DLL into each of them.
Performs Unhooking of DLLs so we can call normal shellcode injection functions without worry.
uses AES encyrption of the shellcode so we can embed the shellcode in our implant without it being detected.
used metasploit to generate shellcode with exitfunc=thread so we dont kill teams process when we exit our meterpreter session.
