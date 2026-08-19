🚀 My DevSecOps Project — Learning by Integrating the Entire Stack

I recently completed a hands-on DevSecOps project where my main goal was not just to learn individual tools, but to understand how different technologies integrate with each other to build a complete CI/CD and cloud deployment workflow.

The project started with infrastructure provisioning and gradually evolved into a complete DevSecOps pipeline:

🔹 1️⃣ Infrastructure as Code — Terraform + AWS EKS
I provisioned the Kubernetes infrastructure on AWS using Terraform, including the EKS environment and supporting resources.

🔹 2️⃣ Testing & Code Quality Pipeline
Created a dedicated Jenkins pipeline for application testing and quality checks using:

SonarQube
OWASP security practices
Quality Gates
Dependency management

🔹 3️⃣ Docker & Container Security Pipeline
Built the application using a Dockerfile, created Docker images, pushed them to Docker Hub, scanned them with Trivy (Aqua Security), and deployed the application directly as a container.

🔹 4️⃣ Kubernetes Deployment Pipeline
Created another Jenkins pipeline for Kubernetes deployment. I used separate YAML manifests for:

Deployment
Service

The application was deployed on Kubernetes and exposed through an AWS Application Load Balancer (ALB).

I also implemented both deployment approaches — Docker container deployment and Kubernetes deployment — to build a stronger foundation in containerization and orchestration.

🛡️ The major focus: DevSecOps

Security was one of the most important parts of this project. I integrated security into the CI/CD workflow using:

✅ SonarQube for code quality and static analysis
✅ OWASP-based security practices
✅ Trivy for container/image vulnerability scanning
✅ Dependency and security checks
✅ Quality Gates to prevent poor-quality code from moving forward

📊 Monitoring, Observability & Tracing

I also worked on the observability side and integrated:

Prometheus → Metrics
Grafana → Dashboards & visualization
Loki → Logs
Jaeger → Distributed tracing
Gmail → CI/CD notifications

🌐 API Integration

Another interesting part was integrating the TMDB API with the application. Instead of relying only on static frontend data, the frontend consumes movie-related data through API calls.

This helped me understand not only DevOps tooling, but also how application → API → container → CI/CD → infrastructure → Kubernetes → monitoring can fit together as one system.

🔧 The most valuable part: Troubleshooting

While building the project, I faced and resolved several real-world issues, including:

• Port conflicts
• Instance type / RAM and resource limitations
• Networking and connectivity problems
• Container deployment issues
• Kubernetes deployment and service issues
• CI/CD integration problems
• Security scan and quality-gate related issues

These problems were actually one of the biggest learning experiences because solving them required understanding why the components were failing, rather than simply following tutorials.

🎯 What I learned most from this project

The biggest takeaway is that DevSecOps is not about knowing Jenkins, Docker, Kubernetes, Terraform, SonarQube, or AWS individually.

It is about understanding how these technologies work together and how security, automation, monitoring, testing, infrastructure, and deployment can become part of one continuous workflow.

This project gave me a much stronger foundation in:

Git → Jenkins → Terraform → AWS/EKS → SonarQube/OWASP → Trivy → Docker → Docker Hub → Kubernetes → ALB → Prometheus → Grafana → Loki → Jaeger → Notifications

Still learning, still breaking things, and still fixing them — but that is exactly where the real learning happens. 🚀
