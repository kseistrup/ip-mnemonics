## IP Mnemonics

Generate a unique mnemonic for any IPv4 address.

Inspired by [@gurno](https://github.com/gurno)'s writeup,
[IP Mnemonics](http://gurno.com/adam/mne/), here's a set of Python scripts
that lets you convert to and from mnemonics:

```sh
$ ip2mne 127.0.0.1
lab-zip-zip-ace
$ ip2mne 127.0.0.1 | mne2ip
127.0.0.1
$ ip2mne 10.0.0.1 172.16.2.3 192.168.4.255
10.0.0.1	arm-zip-zip-ace
172.16.2.3	pal-ban-act-add
192.168.4.255	rat-out-age-all
$ dig a www.google.com +short | ip2mne
sky-eat-shy-fed
```

### Requirements

* Python 3

### Installation

Copy the scripts, `ip2mne` and `mne2ip`, from `src` to a directory in your
`$PATH` and you're all set.
