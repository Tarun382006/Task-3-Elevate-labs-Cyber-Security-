Findings from the vulnerability scan:

  SMB (Multiple Issues) / Windows: This indicates Nessus gathered general data regarding your Server Message Block (SMB) configuration. SMB is the protocol Windows uses for sharing files and printers on a network.
  
  Netstat Portscanner (SSH): Nessus used the system's internal netstat command (likely over an SSH connection) to see which network ports are open and listening for traffic, rather than trying to guess by knocking on every port from the outside.
  
  Host Fully Qualified Domain Name (FQDN) Resolution: This simply means the scanner successfully looked up and resolved the full domain name or computer name of the device being scanned.
  
  Nessus Scan Information: This is a standard administrative log entry. It contains the technical metadata about the scan itself, such as the scanner version, the time it took, and the specific plugin sets used.
  
  Netstat Connection Information: Similar to the portscanner entry, this is a dump of the active network connections and routing tables on the machine at the time of the scan.
  
  OS Identification: Nessus successfully analyzed network responses and system footprints to determine exactly what operating system (and usually which version/build) the machine is running.
  
  OS Security Patch Assessment Failed: Because the scan lacked administrative privileges (as noted above), Nessus was blocked from checking the internal Windows Update logs. Therefore, it couldn't verify if your computer is missing important security patches.


  The scan didnt actually show any serious vulnerability, it just showed the list of things it checked. And the Vulnerability risk was "NONE". I am not sure if anything went wrong here. But this is all I could find.
