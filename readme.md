

# UAC Bypass Vulnerability in Windows Script Host

The Windows Script Host executables suffer from a vulnerability due to a missing embedded manifest. This allows the script host executables to be copied to another system directory and allows a manifest to be applied to the executable. This manifest allows to execute the script host with administrative rights. 

Both ZDI and Microsoft are aware of this issue, expectedly ZDI didn't accept the admission because it's not a remote vulnerability. Surprisingly Microsoft didn't accept the vulnerability because "UAC isn't considered a security boundary".

Only Windows 7 is vulnerable, Windows 8 has a embedded manifest and Windows 10 is untested.
