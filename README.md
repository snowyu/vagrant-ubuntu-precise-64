## About

This script has been ported to Ubuntu 12.04. It will: 

 1. download the Ubuntu 12.04 alternate server (torrent), 64bit iso
 2. ... do some magic to turn it into a vagrant box file
 3. output package.box 

## Usage

    $ sudo ./build.sh

This should do everything you need. If you don't have you must 
have `transmission-cli` installed `sudo apt-get install transmission-cli`
if not. Likewise, `file-roller` (which should be installed by default with
Ubuntu-Desktop, otherwise `sudo apt-get install file-roller` then:

### Kev's notes

"Let's do it all on my **Ubuntu PC**, I said."

Standing on the shoulder's of giants (thanks Carl & Ben) - I have 
modified this `bash` script to work on Ubuntu 12.04 (Precise Pangolin). 
I also modified to download via torrent instead of slow HTTP.

### Ben's notes

Forked Carl's repo, and it sort of worked out of the box. Tweaked 
office 12.04 release: 

 - Downloading 12.04 final release. (Today as of this writing)
 - Checking MD5 to make sure it is the right version
 - Added a few more checks for external dependencies, mkisofs
 - Removed wget, and used curl to reduce dependencies
 - Added more output to see what is going on
 - Still designed to work on Mac OS X :)
    ... though it should work for Linux systems too (maybe w/ a bit of porting)

### Carl's original README

Decided I wanted to learn how to make a vagrant base box.

Let's target Precise Pangolin since it should be releasing soon, I said.

Let's automate everything, I said.

Let's do it all on my macbook, I said.

Woo.
