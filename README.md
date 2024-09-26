# Cybersecurity-Assignment
# DDoS Attack Sequence Diagram

```mermaid
sequenceDiagram
    participant Attacker
    participant BotNet
    participant WebServer
    participant Firewall

    Attacker->>BotNet: Infect multiple systems
    BotNet->>WebServer: Send massive traffic
    WebServer->>Firewall: Overwhelmed by requests
    Firewall->>WebServer: Traffic analysis
    Firewall->>BotNet: IP blocking
    BotNet->>Attacker: Report blocked IPs

## Explanation of the DDoS Attack Sequence

1. **Attacker Infects BotNet:** The attacker infects multiple systems (BotNet) by exploiting vulnerabilities.
2. **BotNet Attacks Web Server:** The BotNet starts sending large amounts of traffic to overwhelm the target server.
3. **Web Server Alerts Firewall:** The server becomes overwhelmed and notifies the firewall.
4. **Firewall Analyzes Traffic:** The firewall analyzes traffic, looking for abnormal behavior.
5. **Firewall Blocks IPs:** The firewall blocks IP addresses identified as part of the attack.
6. **BotNet Reports to Attacker:** After IPs are blocked, the BotNet reports back to the attacker.
