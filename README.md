# azure-pacemaker-agents
A collection of various pacemaker resource agents for use in Azure environments.

## Azure EIP ("External IP")
Update external IP <=> internal IP mappings via Azure API on "start",
and make sure they point back on "monitor". Do nothing on "stop".

## Azure HA ("internal")
Update route tables via Azure API on "start", and make sure
those tables point back on "monitor". Do nothing on "stop".

## HA for Azure VirtualWAN
Update the static routes of a specific Virtual Network
connection via Azure API on "start" to make sure those routes point to us. Check
that those routes still point to us on "monitor". Do nothing on "stop".
