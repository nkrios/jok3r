=====
TODO
=====

BUGS
===============================================================================
* When using --cat-only: [Check 01/total] => total is taking all checks in account
* cmd> java -jar jndiat.jar datasource -v -s 192.168.142.41 -p 7002   
	SEVERE:You must to choose a mandatory command (--sql-shell, --listen-port)  to run this module


IMPROVEMENTS / NEW FEATURES
===============================================================================
* Run custom command
* Session / Restore
* Indicate checks that need a reverse connection (IP reachable from target)


SMARTMODULES / MATCHSTRINGS
===============================================================================
Not done yet:
* impacket smbexec/wmiexec/psexec
* whatweb
* nikto -> too many junk to extract important issues i think
* davscan
* wpseku 
* vbscan
* barmie
* snmpwn



CHECKS TO ADD
===============================================================================


* https://github.com/Coalfire-Research/java-deserialization-exploits/blob/master/OpenNMS/opennms_rce.py
* https://github.com/AlisamTechnology/PRESTA-modules-shell-exploit/blob/master/PRESTA-shell-exploit.pl
* Sharepoint -> https://github.com/TestingPens/SPartan
* check https://bitvijays.github.io/LFF-IPS-P2-VulnerabilityAnalysis.html
* https://github.com/RhinoSecurityLabs/CVEs/tree/master/CVE-2019-0227

* http://pentestit.com/apache-jmeter-rmi-remote-code-execution-vulnerability-poc-cve-2018-1297/
* magento sqli https://github.com/vulhub/vulhub/tree/master/magento/2.2-sqli https://github.com/ambionics/magento-exploits
* VulnX
* Wordpress RCE https://github.com/opsxcq/exploit-CVE-2016-10033

DOCUMENTATION
===============================================================================
* Important note: need to be reachable directly from target for exploit with reverse shell !

sudo docker run -i -t --name jok3r-container -w /root/jok3r -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix --shm-size 2g --net=host koutto/jok3r



SERVICES TO ADD
===============================================================================
* NFS
    * nfsshell (sudo apt-get install libreadline-dev ; make)
* MongoDB
* RPC
    * https://github.com/hegusung/RPCScan.git
* DNS
* LDAP
* MDNS
    * https://github.com/chadillac/mdns_recon
* POP3
* REXEC
* RLOGIN
* RSH
* IMAP




Whatweb:
Summary   : Script, HTML5, Drupal, PHP[7.2.3], HTTPServer[Debian Linux][Apache/2.4.25 (Debian)], X-Powered-By[PHP/7.2.3], PoweredBy[-block], UncommonHeaders[x-drupal-dynamic-cache,x-content-type-options,x-generator,x-drupal-cache], MetaGenerator[Drupal 8 (https://www.drupal.org)], Content-Language[en], Apache[2.4.25], X-Frame-Options[SAMEORIGIN], X-UA-Compatible[IE=edge]
