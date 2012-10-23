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

