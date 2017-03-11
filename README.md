



New-DJBDNS
==========


Hello all,

I am pleased to release this *new* djbdns version 1.06. Djbdns is a
fully-fledged Domain Name System(DNS), originally written by the eminent
author of qmail, Dr. D J Bernstein. This new release is a complete makeover to
the original source(djbdns-1.05) and is meant to make life a lot more pleasant.
The original source is in public-domain since late Dec 2007.

Please see: http://cr.yp.to/distributors.html

Nevertheless, this new release is distributed under the GNU General Public
Licence for good. See ChangeLog for more details.

Installation:
-------------

To install djbdns, say:

    sh>$ ./configure [ --prefix=/usr/local ]
    sh>$ make
    sh># make install

Once installed, on Linux machines add `dnscache' to the system services by
following steps. Note that, if you chose a different install prefix with
`--prefix', use that instead of the default - /usr/local.

    sh># mv /usr/local/bin/dnscached /etc/init.d/dnscached
    sh># chkconfig --add dnscached
    sh># chkconfig --list dnscached

Now you can start the service by

    sh># service dnscached start

OR

    sh># dnscache -D

Consult the dnscache(8) manual page for more help.

Problems:
---------

If you encounter any problems while installing New-DJBDNS OR find bugs in its
working, please send an email to <pj.pandit@yahoo.co.in> describing in detail
about the problem/bug.

Thank you!
