# NexusITSM

**NexusITSM** is a lightweight, agent-based **Automated ITSM Incident Management System** designed to detect client-side issues, generate intelligent tickets, and assign them to the appropriate administrators with minimal manual intervention.

It focuses on **client-level awareness, automation, and reduced incident noise**, making it ideal for small to mid-scale IT environments, labs, and academic use.

---

## 🚀 Key Features

- **Agent-Based Monitoring**
  - Runs on client machines
  - Performs automatic and on-demand system checks
  - Reports health metrics and anomalies to the server

- **Automated Incident Detection**
  - Identifies common system issues (CPU, memory, disk, processes, services)
  - Detects anomalies using rule-based logic

- **Automatic Ticket Generation**
  - Converts detected issues into structured ITSM tickets
  - Prevents duplicate or noisy ticket creation

- **Smart Assignment**
  - Assigns incidents to administrators based on predefined rules
  - Supports round-robin and category-based assignment

- **Client Dashboard**
  - View system health and ticket status
  - Raise manual tickets or queries
  - Track resolution progress

- **Extensible Architecture**
  - Modular agent checks
  - Easy to add new rules, checks, and integrations

---

## 🧩 System Architecture

```
+-------------+        API       +-------------+       API        +-------------+
|   Agent     |  <------------>  |   Server    |  <------------>  |   Client UI |
| (Client OS) |                  | (ITSM Core) |                  | (Dashboard) |
+-------------+                  +-------------+                  +-------------+
```

Agent(Client OS) <-- API --> Server (ITSM Core) <-- API --> Client UI

---

## 🔄 Incident Lifecycle

1. Agent runs scheduled or manual checks  
2. Anomaly detected at client level  
3. Data sent to NexusITSM Server  
4. Server validates and correlates issue  
5. Ticket is created (or merged if similar exists)  
6. Ticket assigned to responsible admin  
7. Admin resolves and updates status  
8. Client dashboard reflects progress  

---

## 🎯 Project Goals

- Reduce manual incident reporting  
- Detect issues before users escalate them  
- Minimize alert and ticket noise  
- Provide client-side context to administrators  
- Serve as a learning-focused yet industry-aligned ITSM system  

---

## 📚 Use Cases

- University labs  
- Startup IT teams  
- Small organizations  
- Internal infrastructure monitoring  
- Academic and interim projects  
