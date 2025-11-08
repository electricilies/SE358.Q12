# Budget Management

## Budget Requirements & Costs

| Component/Task | Detailed Item | Quantity | Unit Cost | Total Cost |
| --- | --- | --- | --- | --- |
| **Personnel Costs** |     |     |     |     |
| Business Analyst | Monthly salary | 1 person × 4 months | $800/month | $3,200 |
| Software Developer | Monthly salary | 4 people × 4 months | $1,000/month | $16,000 |
| QA Tester | Monthly salary | 2 people × 4 months | $700/month | $5,600 |
| UI/UX Designer | Monthly salary | 2 people × 4 months | $750/month | $6,000 |
| Project Manager | Monthly salary | 2 people × 4 months | $1,200/month | $9,600 |
| DevOps Engineer | Monthly salary | 1 person × 4 months | $1,100/month | $4,400 |
| **Infrastructure - Hardware** |     |     |     |     |
| Kubernetes Master Node | Mini PC (16GB RAM, 256GB NVMe) | 1 unit | $250 | $250 |
| Network Switch | 8-port Gigabit managed switch | 1 unit | $45 | $45 |
| UPS Battery Backup | 1000VA UPS for server protection | 1 unit | $80 | $80 |
| Network Cables | Cat6 Ethernet cables (10ft) | 5 cables | $8  | $40 |
| Server Rack/Cabinet | Small 6U wall-mount rack | 1 unit | $60 | $60 |
| **Infrastructure - Storage** |     |     |     |     |
| Backup Storage | 500GB External HDD for backups | 1 unit | $10 | $10 |
| **Infrastructure - Network & Domain** |     |     |     |     |
| Domain Registration | .id.vn domain (1 year) | 1 domain | $3  | $3  |
| SSL Certificate | Let's Encrypt (Free) | 1 certificate | $0  | $0  |
| Static IP Address | Dedicated static IP (if needed) | 4 months | $10/month | $40 |
| Internet Connection | Business internet (100Mbps) | 4 months | $60/month | $240 |
| **Infrastructure - Utilities** |     |     |     |     |
| Electricity | Server power consumption (~300W 24/7) | 4 months | $35/month | $140 |
| Office Space | School, Work from home |     | $0  | $0  |
| **Software & Services** |     |     |     |     |
| Container Registry | Github container registry (GHCR) |     | $0  | $0  |
| Monitoring Service | Self-hosted Prometheus + Grafana |     | $0  | $0  |
| Log Management | Self-hosted Grafana Loki |     | $0  | $0  |
| Database | PostgreSQL (self-hosted) |     | $0  | $0  |
| Cache System | Redis (self-hosted) |     | $0  | $0  |
| Identity and Access Management | Keycloak (self-hosted) |     | $0  | $0  |
| CI/CD Pipeline | GitHub Actions (free tier) |     | $0  | $0  |
| Message Queue | RabbitMQ/Kafka (self-hosted, if needed) |     | $0  | $0  |
| Reverse Proxy/Ingress | Traefik/Nginx Ingress Controller |     | $0  | $0  |
| **Development Tools & Licenses** |     |     |     |     |
| IDE Licenses | VSCode, Neovim |     | $0  | $0  |
| Design Software | Figma (Free tier) |     | $0  | $0  |
| API Testing Tool | Postman (Free tier), Bruno |     | $0  | $0  |
| Project Management | Jira Software Free |     | $0  | $0  |
| Documentation | VitePress with Github Pages |     | $0  | $0  |
| Communication | Facebook Messenger, Telegram |     | $0  | $0  |
| Version Control | Git, GitHub (Free) |     | $0  | $0  |
| Database Management | DBeaver Community |     | $0  | $0  |
| **Testing & QA** |     |     |     |     |
| Load Testing Tool | Grafana K6 (open-source) |     | $0  | $0  |
| Browser Testing | Playwright with CI |     | $0  | $0  |
| Test Coverage | Codecov (Free for open source) |     | $0  | $0  |
| Security Scanning | SonarQube Community/Cloud (Free tier) |     | $0  | $0  |
| API Documentation | Swagger/OpenAPI (self-hosted) |     | $0  | $0  |
| **Documentation & Assets** |     |     |     |     |
| Diagram Tools | PlantUML |     | $0  | $0  |
| Image Optimization | TinyPNG, ImageOptim (Free tools) |     | $0  | $0  |
| **Training & Learning** |     |     |     |     |
| Online Courses | YouTube, freeCodeCamp, MDN |     | $0  | $0  |
| Technical Documentation | Official docs (PostgreSQL, K8s, etc.) |     | $0  | $0  |
| **Marketing & Launch** |     |     |     |     |
| Landing Page Hosting | Github Pages (Static site) |     | $0  | $0  |
| Email Service | Self-hosted or Gmail SMTP |     | $0  | $0  |
| SEO Tools | Google Search Console (Free) |     | $0  | $0  |
| **Legal & Compliance** |     |     |     |     |
| Business Registration | Company registration fees (if applicable) | 1 time | $10 | $10 |
| Terms & Privacy Policy | Legal document templates (online) |     | $0  | $0  |
| GDPR Compliance Tools | Cookie consent banner (free libraries) |     | $0  | $0  |
| **Contingency & Miscellaneous** |     |     |     |     |
| Hardware Replacement | Reserve for hardware failure | Buffer |     | $300 |
| Software Emergency | Unexpected paid service needs | Buffer |     | $150 |
| Team Building | Team activities/meals (pizza parties) | 4 events | $50 | $200 |
| Office Supplies | Whiteboards, markers, notepads, etc. | Miscellaneous |     | $100 |
| Emergency Fund | General contingency (~5% of operational) |     |     | $100 |
| **Subtotal (Operational Costs)** |     |     |     | **$1,768** |
| **Subtotal (Personnel Costs)** |     |     |     | **$44,800** |
| **Grand Total** |     |     |     | **$46,568** |

## Prompt

```
I have given you context about my project including use cases, function list. You will create budget management in the bottom-up method for Electricilies - Website for Selling Electronic Products. This is just a university project, 4 members, so don't think this is for a big company. We use github and github action, deploy on selfhost kubernetes (not cloud), office at school or work from home, free document, grafana and prometheus stack, testing (Playwright, K6, Codecov, SonarQube)
```