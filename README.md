SecureCentos
==============

This project contains configuration files for services installed in secure 
way in Centos distro. Could be also helpful on some other Linux distributions.

If You ever come around the world of Centos configuration - check Your
config files with those from this repo. Maybe You'll find that something
could be more secure. 

Remember:
--------------

  * Do not disable Selinux - ever! If You have any issues with that - use 
  "sealert -a" to generate report about blocked events.
  * Do not disable iptables. Even on backend machines inside secure network.
  There is no such a place called "secure network".
  * Filter outgoing traffic on iptables.
  * Turn off SSH logging with passwords - keys are enough
  * Turn of SSH logging for root
  * Move SSH service from 22 port to some higher, unprivileged
  * Allow for SSH logging only for specific user group - will be easier
  (and more secure) to manage users
  * Use sudo. 
  * Use cgroups to preserve resources for mission critical services
  * Remember about restricted shells
  * Do NOT use pure FTP. Use sFTP instead (or FTPs). Could be also
  SCP over SSH via restricted shell (rssh)

License:
--------------

Whatever - those configurations are not subject to any license ;)