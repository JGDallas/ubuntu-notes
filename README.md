# ubuntu-notes
Unable to lock the administration directory (/var/lib/dpkg/) is another process using it?

https://askubuntu.com/questions/15433/unable-to-lock-the-administration-directory-var-lib-dpkg-is-another-process

sudo fuser -vik -TERM /var/lib/dpkg/lock /var/lib/dpkg/lock-frontend /var/lib/apt/lists/lock
sudo dpkg --configure --pending

