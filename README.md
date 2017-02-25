## IP Mnemonics

Generate a unique mnemonic for any IPv4 address.

Inspired by Adam Gurno's writeup, [IP Mnemonics](http://gurno.com/adam/mne/),
here are a set of Python scripts that let you convert to and from mnemonics:

```sh
$ ip2mne 127.0.0.1
lab-zip-zip-ace
$ ip2mne 127.0.0.1 | mne2ip
127.0.0.1
$ ip2mne 10.0.0.1 172.16.2.3 192.168.4.255
10.0.0.1	arm-zip-zip-ace
172.16.2.3	pal-ban-act-add
192.168.4.255	rat-out-age-all
```
