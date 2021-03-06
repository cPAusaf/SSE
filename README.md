SSE
================

Exim email information utility for cPanel servers

Usage
--------------

**# perl <(curl -s https://raw.githubusercontent.com/cPanelTechs/SSE/master/sse.pl) [options]**


**Current Checks Impliemented:**

- Print current exim queue.
- Check for custom /etc/mailips, /etc/mailhelo, and /etc/reversedns.
- Check if port 26 is enabled.
- Check if mail IPs are blacklisted
- Show reverse DNS for mail IPs
- Check for SPF and DKIM records
- Check if nobody user is prevented from sending mail.
- Check server's PHP handler (PHP5 only at this time.)

**[With --domain or -d option]**

- Check if domain exists on the server.
- Check if the user account is suspended.
- Check if domain is identical to hostname.
- Check if domain is in remote or local domains.
- Check if domain resolves locally to server.
- Check if domain has any virtual filters.

**[With --email or -e option]**

- Check if e-mail exists on server.
- Check if e-mail has forwarders.
- Check if e-mail has an autoresponder enabled.
- Check if mailbox has filters.

**[With -s option]**

- View summary of email that has been sent from the server

**[With -b option]**

- Check Main IP and IPs in /etc/ips for blacklistings

