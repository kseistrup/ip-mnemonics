## IP Mnemonics

Generate a unique mnemonic for any IPv4 address.

Inspired by [@gurno](https://github.com/gurno)'s writeup,
[IP Mnemonics](http://gurno.com/adam/mne/), here's a Python scripts
that lets you convert to and from mnemonics:

```sh
$ ipmne 10.0.0.1
10.0.0.1	arm-zip-zip-ace
$ ipmne 127.0.0.1
127.0.0.1	lab-zip-zip-ace	localhost
$ ipmne 10.0.0.1 172.16.2.3 192.168.4.255
10.0.0.1	arm-zip-zip-ace
172.16.2.3	pal-ban-act-add
192.168.4.255	rat-out-age-all
$ dig a www.google.com +short | ipmne
216.58.212.100	sky-eat-shy-hog	lhr35s06-in-f100.1e100.net
$ ipmne www.google.com
216.58.212.100	sky-eat-shy-hog	www.google.com
$ ipmne --format '{mnemonic}' www.google.com
sky-eat-shy-hog
```

### Requirements

* [Python 3](https://www.python.org/)
* [dnspython](http://www.dnspython.org/) (optional)

### Installation

Copy the script, `ipmne`, from `src` to a directory in your
`$PATH` and you're all set.

:smile:
