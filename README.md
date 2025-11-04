Purpose
A tiny, lab-only DLL provided to help test DLL-injection workflows and basic injection tooling in a controlled pentesting environment. When invoked correctly the DLL will attempt to launch calc.exe so you can confirm execution and process injection behavior.

Important — legal & safety: Use this repository only on systems you own or where you have explicit written permission to test. Never run these tests on production or third-party systems. The author is not responsible for misuse.

Quick test (run in Windows CMD)

Use the exact command below (replace the path and exported function name as needed):

rundll32.exe "PATH\calculator.dll",EntryPoint


Example:

rundll32.exe "C:\lab\dlls\calculator.dll",EntryPoint


If the DLL is correct and the exported function exists and runs, the Windows Calculator (calc.exe) should open — this confirms the DLL executed.
