# My site by IP Address
## GitLab and GitHub public Projects/Repositories
The
[gitlab.com/aws-lam/aws](https://gitlab.com/aws-lam/gci)
Project is a clone of the
[github.com/LAMurakami/aws](https://github.com/LAMurakami/gci)
Repostory.  My
[gitlab.com/LAMurakami](https://gitlab.com/LAMurakami)
account was created so that Projects can be cloned using https without
authentication over IPv6 as well as IPv4 unlike the
[github.com/LAMurakami](https://github.com/LAMurakami)
Repostories that can only be accessed over IPv6 with the
[IPv6 only workaround.](https://lamurakami.github.io/blog/2024/06/05/Access-GitHub-com-from-an-instance-without-a-public-IPv4-address.html)

## by IP Address website
[https://gci.lam1.us](https://gci.lam1.us)

[https://lam3.freeddns.org](https://lam3.freeddns.org)
[lam1ak.duckdns.org](https://lam1ak.duckdns.org)
Dynamic Domain Name Service subdomain possibly being served by the instance.

This repo contains content in the html folder and an apache2 configuration
that can be implemented with:

 cd /var/www; git clone https://gitlab.com/aws-lam/gci.git

 sudo ln -s /var/www/gci/gci_apache2.conf /etc/apache2/sites-available/000-gci.conf

 sudo a2ensite 000-gci

 sudo systemctl reload apache2

If the repo contents are installed in a location other than /var/www
the path in the configuration and in the instuctions would have to be modified.
