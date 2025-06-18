-   **Cybersecurity Incident Report:**

# **Network Traffic Analysis**

| Part 1: Provide a summary of the problem found in the DNS and ICMP traffic log. |  |
| :---- | :---- |
| The UDP protocol reveals that: This is based on the results of the network analysis, which show that the ICMP echo reply returned the error message: UDP port 53 unreachable. The port noted in the error message is used for: Port 53 is used for DNS service. The most likely issue is:The website did not reach the DNS server because no service was listening on receiving DNS port. |  |
|  |  |

| Part 2: Explain your analysis of the data and provide at least one cause of the incident. |
| :---- |
| Time incident occurred:1:24 p.m., 32.192571 seconds. Explain how the IT team became aware of the incident:The IT team received a message from several clients that the destination port was unreachable. Explain the actions taken by the IT department to investigate the incident:They used the tcpdump command to check for traffic in the service port and destination port. Note key findings of the IT department's investigation (i.e., details related to the port affected, DNS server, etc.): They found that port 53 is unreachable ,DNS service is affected. Note a likely cause of the incident:The DNS server may have crashed due to high network traffic or the firewall may have rejected packets from port 53\. |

 

 

