# Description
The endpoint is periodically accessing an external fixed-IP address that its peers rarely use. Access to this external IP address has occurred repeatedly over many days. This connection pattern is consistent with malware connecting to its command and control server for updates and operating instructions.
# Attacker's Goals
Communicate with malicious code running on your network enabling further access to the endpoint and network, performing software updates on the endpoint, or for taking inventory of infected machines.
# Investigative Actions
Identify if the IP address belongs to a reputable organization or an asset used in a public cloud.
Identify if the source of the traffic is malware. If the source of the traffic is a malicious file, Cortex XDR Analytics also raises a malware alert for the file on the endpoint. Malware may contact legitimate IP addresses, therefore check for unusual apps used, or unusual ports or volumes accessed.
View all related traffic generated by the suspicious process to understand the purpose.
Look for other endpoints on your network that are also contacting the suspicious IP address.
Examine file-system operations performed by the process to look for potential artifacts on infected endpoints.
