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
