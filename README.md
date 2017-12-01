# Linux CLI cheatsheet

### A reference tool for maintaining and searching a cheatsheet for Linux commands

Summary:
---------------------
I use this to quickly look up Linux commands I run frequently but don't want to remember or type.  The cheatsheet file itself is just an example.  Please modify your own cheatsheet as you see fit.  

Setup:
---------------------
1. Copy these files to a local directory. For exaple:
```bash
mkdir ~/.cheatsheet && cd ~/.cheatsheet && git clone https://gist.github.com/c0reysc0tt/ccde4ffd1e5ff740569f5cd9700a4262 .
```

2. Copy the contents of of the included .bashrc snippet to your own .bashrc or .bash_profile. For example:
```bash
cat .bashrc >> ~/.bashrc && source ~/.bashrc
```

### .bashrc notes:
- Make sure the `CHEATDIR` variable matches the location where you cloned the repo.
- If you plan to use your cheatsheet on multiple systems but don't want to use Git, consider putting it in a Dropbox or Google Drive folder that automatically syncs with a cloud service.
- The `thecheat` function is optional.  See below for additional dependencies and usage.

Usage:
---------------------
Use `cheat <word>` to search the cheatsheet for a word.  Results will look like this:

![alt text](https://gist.githubusercontent.com/c0reysc0tt/ccde4ffd1e5ff740569f5cd9700a4262/raw/8b02338adcafcae800ee9bf3cc59f17bff7d1251/screenshot_cheat.png "cheat cron")


To have your results delivered by a colorful ASCII version of The Cheat from Homestar Runner, type `thecheat <word>` instead.  This requires that both **cowsay** and **lolcat** are installed, and you'll need to copy the included thecheat.cow file into your cowsay cows folder.  On my Mac, it looks like this:
```bash
cp thecheat.cow /usr/local/Cellar/cowsay/3.04/share/cows/
```

![alt text](https://gist.githubusercontent.com/c0reysc0tt/ccde4ffd1e5ff740569f5cd9700a4262/raw/8b02338adcafcae800ee9bf3cc59f17bff7d1251/screenshot_thecheat.png "thecheat yum")

Editing the cheatsheet:
---------------------
You can quickly edit the cheatsheet file using `vicheat`.  I chose that name to follow the same convention as visudo, but you can edit the alias in the .bashrc file if something else makes more sense to you.  


## I hope this is useful to some people out there, and I welcome your feedback!  Happy cheating!
