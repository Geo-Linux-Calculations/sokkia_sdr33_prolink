Sokkia SDR 33 Prolink
=====================

This is part https://github.com/Geo-Linux-Calculations/python-sdr33triangle of connecting tools.  
This fork connecting tools https://github.com/r-barnes/sdr33_triangulation  
This repository contains connecting tools of SDR33 data logger file.  

Windows
=======

Unzip sokkia_prolink115.zip
Run Setup.exe
Run ProLink.

Linux
=====

Configure "device"

```
stty "speed" -F "device"
```
Example and info:
```
stty 9600 -F /dev/ttyS0
stty -a -F /dev/ttyS0
```

Get data

```
cat|pv "device" > you.sdr
```
Example:
```
pv /dev/ttyS0 > you.sdr
```

Send data

```
cat|pv you.sdr > "device"
```
Example:
```
cat you.sdr > /dev/ttyS0
```

Links
=====
https://github.com/r-barnes/sdr33_triangulation  
https://github.com/Geo-Linux-Calculations/python-sdr33triangle  
https://github.com/Geo-Linux-Calculations/sokkia_sdr33_prolink  
https://github.com/Geo-Linux-Calculations/sokkia_sdr33_manual  

Mantainer
=========
zvezdochiot  
2019
