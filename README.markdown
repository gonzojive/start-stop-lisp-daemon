# start-stop-lisp-daemon

This is 2 shell scripts and a local version of detachtty that can be
used in combination with screen to administer lisp applications.

#Instructions

Installation: Put the 'lisp-daemon' file into /etc/init.d and
'start-stop-lisp-daemon' into /usr/local/bin.  Next compile and
install detachtty (see the detachtty directory.  Note that you need
the local version of detachtty to work; Ubuntu's/Debian's is out of
date.

Now define a bunch of lisp images in /etc/lisp-start.d/.  A typical
example of this kind of file is in 'example-server'

run /etc/init.d/lisp-start example-server start to start.

