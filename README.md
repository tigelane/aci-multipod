# aci-multipod
<P>
There are four files here in two logical groups.   The two text files are the running configs of my IPN Nexus 9200 series standlone switches.  Use these as example to build up your own IPN devices.  Key areas to look at are setting up PIM, DHCP-Relay, MTU of 9150, and OSPF.
<P>
<B>UPDATE DEC 2016</B>
<P>
<I>I have updated my IPN config to use an optional (but recommended) vrf just for the multipod stuff.  Please review the running config files in version 2 in this repo.  Also note some PIM commands now moved to the dedicated vrf context.</I>
<P>
<HR>
<P>
The two python scripts are those used in my own lab to setup the OSPF adjacency to IPN (<B>mpod-base.py</B>) and the other to setup the physical front-panel ports (i.e complete the MP-BGP control plane) on the ACI fabric used by the spines towards the IPN (<B>mpod-phys.py</B>).  Please note that the scripts use values that are <b>specific to my own setup</b>.  You will need to edit them to match the ports, ip addresses and settings in your own environment.  


