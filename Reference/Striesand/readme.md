## Striesand Server

* *Nginx* powers a password-protected and encrypted Gateway that serves as the starting point for new users. The Gateway is accessible over SSL, or as a Tor hidden service.

* Beautiful, custom, step-by-step client configuration instructions are generated for each new server that Streisand creates. Users can quickly access these instructions through any web browser. The instructions are responsive and look fantastic on mobile phones.

* The integrity of mirrored software is ensured using SHA-256 checksums, or by verifying GPG signatures if the project provides them. This protects users from downloading corrupted files.

* All ancillary files, such as OpenVPN configuration profiles, are also available via the Gateway.

* Current Tor users can take advantage of the additional services Streisand sets up in order to transfer large files or to handle other traffic (e.g. BitTorrent) that isn't appropriate for the Tor network.

* A unique password, SSL certificate, and SSL private key are generated for each Streisand Gateway. The Gateway instructions and certificate are transferred via SSH at the conclusion of Streisand's execution.

* Distinct services and multiple daemons provide an enormous amount of flexibility. If one connection method gets blocked there are numerous options available, most of which are resistant to Deep Packet Inspection.

* All of the connection methods (including direct OpenVPN connections) are effective against the type of blocking Turkey has been experimenting with.

* OpenConnect/AnyConnect, OpenSSH, OpenVPN (wrapped in stunnel), Shadowsocks, Tor (with obfsproxy and the obfs4 pluggable transport), and WireGuard are all currently effective against China's Great Firewall.

* Every task has been thoroughly documented and given a detailed description. Streisand is simultaneously the most complete HOWTO in existence for the setup of all of the software it installs, and also the antidote for ever having to do any of this by hand again.

* All software runs on ports that have been deliberately chosen to make simplistic port blocking unrealistic without causing massive collateral damage. OpenVPN, for example, does not run on its default port of 1194, but instead uses port 636, the standard port for LDAP/SSL connections that are beloved by companies worldwide.



## DeploymentSamples

Contains samples on how to use the Resource ARM Templates. 

### Reference Design for Striesand Appliance

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FDamianFlynn%2Farm%2Fmaster%2FReference%2FWiregurd%2FrefWireguard.json" target="_blank">

  <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FDamianFlynn%2Farm%2Fmaster%2FReference%2FWireguard%2FrefWireguard.json" target="_blank">
  <img src="http://armviz.io/visualizebutton.png"/>
</a>