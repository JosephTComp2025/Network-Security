By adding Security Onion to monitor traffic within my network, Suricata detected multiple SSH brute‑force attempts originating from a single internal IP address. I then used the Zeek logs inside Security Onion to confirm these short‑lived SSH sessions and validate the brute‑force activity. This alert was a true positive.
This attack was simulated using a Parrot OS attacker VM inside the internal network, targeting the Security Onion management interface. There were zero successful authentication attempts and no signs of compromise on the target system.
In the real world, the next steps to contain this attack would include blocking the offending IP address at the network firewall, enabling rate‑limiting or lockout policies on SSH (MITRE ATT&CK M1036), confirming MFA is enabled (MITRE ATT&CK M1027), reviewing system logs for unauthorized access, and validating the integrity of critical resources within the environment.
Although I have used Suricata in a standalone lab before, it was great to see how Suricata signatures and Zeek logs worked together inside Security Onion to validate and correlate this attack.














