# att-udmpro-maintenance

One purpose of this repository is to point at the various resources necessary to use Unifi Dream Machine Pro from Ubiquiti on AT&T's fiber optic network, without using an AT&T-supplied residential gateway (in my case, the BGW210-700). The other purpose is to share the scripts/methods I am using to keep it going, so that a reboot or a firmware update on the UDMPro does not take my internet with it.

## Certificates

Reddit user u/Streiw shared his take on getting telnet access to the BGW210-700:
- https://www.reddit.com/r/ATT/comments/g59rwm/bgw210700_root_exploitbypass/

He posted all of his instructions:
- https://pastebin.com/SUGLTfv4

But that only got the mfg.dat file. You also need the contents of the /etc/rootcert folder to be able to decode the contents.
- `tar cf /www/att/images/cert.tar /etc/rootcert/`

Download http://192.168.1.254/images/cert.tar to your local mchine.
