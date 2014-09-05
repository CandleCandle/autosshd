


autosshd
========

Adapted from https://gist.github.com/haku/6322759


Install
-------

```bash
hostname=<insert hostname here>
git clone https://github.com/CandleCandle/autosshd.git autosshd
cd autosshd
sudo ./install $hostname
sudo vim /etc/autosshd-$hostname/ssh_config
sudo ssh -F /etc/autosshd-$hostname/ssh_config tunnel
sudo service autosshd-$hostname start
```

And then install `/etc/autosshd/id_rsa.pub` at target.


