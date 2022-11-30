# Description
A remotely triggered service initiated a command execution in a PsExec-like manner by a host that rarely triggers services to other remote hosts.
# Attacker's Goals
Perform lateral movement to new hosts to expand the foothold within a network.
# Investigative Actions
Investigate the processes being spawned on the host for malicious activities.
Correlate the RPC call from the source host and understand which software initiated it.