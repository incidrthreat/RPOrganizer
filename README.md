# About RPOrganizer

`RPOrganizer.exe` is a helper tool created with .NET Core to help organize (as a first filter) ROPs commands in order to create ROP chains.
It receives as input a file generated by RP++ (https://github.com/0vercl0k/rp)

```bash
PS C:\Users\daniel\Desktop\RP> .\rp-win-x86.exe -f "somedll.dll" -r 5 > rop.txt
```

Usage:

```bash
PS C:\Users\daniel> .\RPOrganizer.exe -i C:\Temp\ROP.txt -o C:\Temp\Output.txt
[+] Loaded 195983 gadgets...

[!] Found 0 "DEREF" gadgets...
[!] Found 123 "XCHG" gadgets...
[!] Found 15 "MOV" gadgets...
[!] Found 30 "ADD" gadgets...
[!] Found 2 "SUB" gadgets...
[!] Found 3638 "POP" gadgets...
[!] Found 3 "NEG" gadgets...
[!] Found 66 "INC" gadgets...
[!] Found 64 "DEC" gadgets...
[!] Found 17007 "RET" gadgets...
[!] Found 0 "WRITE" gadgets...
[!] Found 67 "GET ESP" gadgets...

[+] Output saved to C:\Temp\Output.txt
```

*It was created during my studies for OSED and it's far from it's optimal stage.*
