# Cybersecurity-Assignment
## DDoS Attack Sequence Diagram

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
