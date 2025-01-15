```mermaid
flowchart TD;
    subgraph Improved Web Infrastructure
        LB1[Load Balancer 1: HAProxy] -->|Traffic| WS[Web Server: Nginx]
        LB2[Load Balancer 2: HAProxy] -->|Traffic| WS
        WS --> AS[Application Server]
        AS --> DB[(Database: MySQL)]
    end
