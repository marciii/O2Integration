# O2Integration
Collection of scripts and tools for integrating the whole O2 system on the HLT dev cluster

hosts.cfg : DDS hosts file (describes the available nodes for distribution via DDS ssh plugin).

topology.xml : DDS topology file (describes the topology and cmd options for all devices).

# Usage

* alienv enter O2/latest
* dds-server  start  –s
* dds-submit  --rms ssh --config  hosts.cfg
* dds-topology --activate topology.xml


* dds-server stop

tasks output  is written to /tmp/dds_wn_dir localy on each node
