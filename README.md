pia
==========
- Designed for debian and arch based linux.
- Update openvpn configuration files using maximum security configuration.
- Instant connections with secure storage of VPN password.
- Forward ports.
- Change DNS to PIA secure leak-proof DNS servers.
- Use firewall to block all non-tunnel traffic

dependencies
==========
- openvpn
- ufw

Installation:
==========

Run 'sudo make install' in the pia directory.
pia will now be installed and can be run with 'pia'.
	
Usage
==========
	Usage: ./pia.sh [Options]

	-s	- Server number to connect to
	-l	- List available servers.
	-u	- Update PIA openvpn files before connecting.
	-p	- Forward a port.
	-n	- Change to another random port.
	-d	- Change DNS servers to PIA.
	-f	- Enable firewall to block all traffic apart from tun0
	-v	- Display verbose information.
	-h	- Display this help.

	Examples: 
	pia -dps 24 	- Change DNS, forward a port and connect to Switzerland.
	pia -nfv	- Forward a new port, run firewall and be verbose.
