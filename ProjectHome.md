**Project moved to https://github.com/quarkslab/quarkspwdump**


Quarks PwDump is a native Win32 tool to extract credentials from Windows operating systems.

It currently extracts :

  * Local accounts NT/LM hashes + history
  * Domain accounts NT/LM hashes + history
  * Cached domain password
  * Bitlocker recovery information (recovery passwords & key packages)

Supported OS : XP/2003/Vista/7/2008/8


---


Bitlocker and domain accounts information are extracted offline from NTDS.dit. It's not currently full offline mode cause the tool is dynamically linked with ESENT.dll which differs between Windows version (see README.txt for details).

Local account and cached information are extracted live from SAM and SECURITY hive in a proper way and without code injection or service installation.

In all cases, the tool must be executed on the targeted machine with administrator privileges.

The project is still in beta test and we would really appreciate to have feedbacks or suggestions/comments about potential bugs.