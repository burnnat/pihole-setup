# pihole-setup

Because Pi-Hole will be used as a DHCP server, be sure to set a static IP address for this Raspberry Pi in file `/etc/dhcpcd.conf`:

    interface eth0
    static ip_address=192.168.2.4/21
    static routers=192.168.2.1
    static domain_name_servers=192.168.2.4 1.1.1.1 1.1.0.1

