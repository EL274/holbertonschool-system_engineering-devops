```mermaid
flowchart TD;
    [User] → [DNS: www.foobar.com → 8.8.8.8] → [Server]
                                           │
                                           ├── [Nginx (Web Server)]
                                           │       │
                                           │       ├── Serves static files
                                           │       └── Proxies to Application Server
                                           │
                                           ├── [Application Server]
                                           │       └── Runs application code
                                           │
                                           └── [MySQL (Database)]
                                                   └── Stores and retrieves data
```
