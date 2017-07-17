# mibank
Collection of Management Information Base (MIB)

## Building the MIBs into list of identifiers
For using with [snmpdump](https://github.com/schoenw/snmpdump) program to extract SNMP messages,
we need to convert MIBs file into list of identifiers
using [smidump](https://linux.die.net/man/1/smidump) program.

For example, generate identifiers for standard MIBs:
```
smidump -k -f identifiers -o MIB-DB iana/* ietf/* irtf/*
```

## Reference
* https://www.ibr.cs.tu-bs.de/projects/libsmi/
* https://github.com/simonjj/SnmpMibs.git
* http://www.circitor.fr/Mibs/Mibs.php
