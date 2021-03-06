.. image:: ../_static/openl2m_logo.png

===================
Create the Switches
===================

Adding switches
===============

From Admin, click on Switches, or click the "+ Add" option

Configure the name to show in the menu (does not need to be the switch hostname)
Add the IP v4 address or resolvable DNS name, and the SNMP profile as a minimum.
If you want to allow 'show/display' commands, you need to add a Netmiko (SSH)
profile as well.

Note: switches will only show in the list if their status is active,
and they have an SNMP Profile applied! Likewise, if a switch does not have
a Netmiko profile, interface commands and global commands options will not show.

If a switch is marked Read-Only, no user (not even admin), can change settings
on the switch. However, if commands are configured, they can be executed.
This is useful for e.g. routers.

The Default View setting defines the opening tab when a user clicks on the
switch. Setting this to Details is useful for routers, so that ARP and
LLDP information shows immediately. Note that it then take a little longer
to render the page, due to the extra SNMP data that needs to be read
from the device.

The Bulk Edit setting is enabled by default. If disabled (un-checked),
this switch will not allow multiple interfaces to be edited at once.

You can add any switch many times, with the same IP address but a
different name. However, the combination of the name and ip address
needs to be unique.
