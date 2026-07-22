# ALU Web Stack

## HTTPS/SSL and DNS Subdomains (https_ssl/)

Configures DNS A records for www, lb-01, web-01, and web-02 subdomains, and includes a script (0-world_wide_web) using dig and awk to audit these records.

### Why secure your website traffic?

Without HTTPS, traffic travels as plain text and can be intercepted or tampered with. SSL/TLS encrypts the connection and verifies server identity.
