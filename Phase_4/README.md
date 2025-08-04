## 📌 Phase 4: Monitoring & Observability (Real-time Feedback)

Monitoring ensures we have visibility into both **system-level performance** and **application health** post-deployment:

- Set up **Node Exporter** on all EC2 instances to track CPU, memory, disk usage
- Connected Prometheus for real-time data scraping
- Built **Grafana dashboards** to visualize system performance
- Implemented **Blackbox Exporter** to monitor HTTP endpoints for:
  - Website uptime
  - Latency
  - TLS/SSL validity

🎯 *Goal*: Provide 360° visibility of the deployed environment to quickly identify and respond to issues.


![Pipeline Architecture](https://github.com/Maverick7t/Devops_project/raw/main/Phase_4/Screenshot%202025-08-04%20151312.png)
![Pipeline Monitoring](https://github.com/Maverick7t/Devops_project/blob/main/Phase_4/Screenshot%202025-08-04%20152256.png)

