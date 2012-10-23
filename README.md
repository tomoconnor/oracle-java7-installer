oracle-java7-installer
======================

Breaking the Oracle Terms of Service in the nicest possible way.

Until very recently, it was possible to get sun-java7-jdk packages directly from Ubuntu.  Then Oracle changed their TOS.

Then someone made an installer, which was *ok*.. But I wanted a debian package format.

So, all you need to do is:

For Java 7 u7:

1. Head to http://www.oracle.com/technetwork/java/javase/downloads/jdk7u7-downloads-1836413.html

2. Download the jdk-7u7-linux-x64.tar.gz file

3. Drop that file in src/var/cache/oracle-jdk7-installer/jdk-7u7-linux-x64.tar.gz

4. run info/bin/build-deb

5. Install the resulting deb file as you wish.

The biggest reason for doing it this way rather than using http://www.webupd8.org/2012/06/how-to-install-oracle-java-7-in-debian.html is because this way gives  you a fat .deb file containing java, so you can install it in places that might not have connectivity (or have slow connectivity).

Also, Oracle will probably cripple the webupd8 method at some point, probably by putting a captcha in front of the downloads page.  Wouldn't surprise me.  The advantage of doing it this way is you do it once, update the deb build environment.  Build the deb, install it.  Done. 