`Usage Notes`

All commands (download of the installer via wget excluded) have to be executed as root or with sudo because they require administrative access to package managers, service commands and directories (eg the /etc/squid directory) where elevated permissions are required.

If you get a SSL error while trying to download the installer file please append `--no-check-certificate` after wget but before the link to the SPi installer file. In order to avoid similar issues in the future you can simply install the ca certificate bundle via your OS package manager. To make the installer work on systems without ca certificate bundles the installer is already using the `--no-check-certificate` flag internally for the download of the different squid.conf configuration files off the GitHub servers. 

`CentOS`

CentOS 5

Run the following one line command to download the SPI installer file to your CentOS 5 server, execute it and let it install and configure Squid (after that the SPI installer file will be removed from your server):

`wget https://raw.githubusercontent.com/MrFrazSultan/Squid-NP/master/spi && bash spi -rhel5 && rm spi`

CentOS 6

Run the following one line command to download the SPI installer file to your CentOS 6 server, execute it and let it install and configure Squid (after that the SPI installer file will be removed from your server):

`wget https://raw.githubusercontent.com/MrFrazSultan/Squid-NP/master/spi && bash spi -rhel6 && rm spi`

CentOS 7

Run the following one line command to download the SPI installer file to your CentOS 7 server, execute it and let it install and configure Squid (after that the SPI installer file will be removed from your server):

`wget https://raw.githubusercontent.com/MrFrazSultan/Squid-NP/master/spi && bash spi -rhel7 && rm spi`


`Debian`

Debian "Squeeze" 6 & Debian "Wheezy" 7

Run the following one line command to download the SPI installer file to your Debian 6 or 7 server, execute it and let it install and configure Squid (after that the SPI installer file will be removed from your server):

`wget https://raw.githubusercontent.com/MrFrazSultan/Squid-NP/master/spi && bash spi -debian && rm spi`

Debian "Jessie" 8

Run the following one line command to download the SPI installer file to your Debian 8 server, execute it and let it install and configure Squid (after that the SPI installer file will be removed from your server):

`wget https://raw.githubusercontent.com/MrFrazSultan/Squid-NP/master/spi && bash spi -jessie && rm spi`

`Ubuntu 18`

Run the following one line command to download the SPI installer file to your Ubuntu server, execute it and let it install and configure Squid (after that the SPI installer file will be removed from your server):

`wget https://raw.githubusercontent.com/MrFrazSultan/Squid-NP/master/spi && bash spi -ubuntu && rm spi`

`Fedora`

Run the following one line command to download the SPI installer file to your Fedora server, execute it and let it install and configure Squid (after that the SPI installer file will be removed from your server):

`wget https://raw.githubusercontent.com/MrFrazSultan/Squid-NP/master/spi && bash spi -fedora && rm spi`

The SPI installer will do everything by itself. You will only be asked for your desired username and password for the first authorized proxy user.

Use Port `443` Which is HTTPS Port or `80` Which is HTTP Port.

Originally Posted By [Hidden Refuge](https://github.com/hidden-refuge/spi/)
