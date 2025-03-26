# `~/profile.tf`

```hcl
# Cloud Solutions Architect | FinOps Specialist | Infrastructure Expert

resource "profile" "about_me" {
  name    = "Your Name"
  role    = "Cloud Solutions Architect & FinOps Specialist"
  focus   = "Turning cloud chaos into elegant, cost-effective infrastructure"
  based   = "Location (Optional)"
  
  expertise = [
    "GCP & AWS architecture at enterprise scale",
    "Infrastructure cost optimization & FinOps implementation",
    "Spacelift platform specialist",
    "Terraform/OpenTofu infrastructure design"
  ]
}

# What I do best

resource "services" "offerings" {
  architecture = "Design cloud solutions that balance performance, cost, and security"
  optimization = "Reduce cloud spend by 20-40% while improving performance"
  automation   = "Build CI/CD pipelines that make infrastructure changes safe and predictable"
  consulting   = "Provide expert guidance on cloud infrastructure decisions"
}

# Tools I use daily

resource "toolchain" "favorites" {
  cloud        = ["GCP", "AWS"]
  iac          = ["Terraform", "OpenTofu", "Ansible"]
  containers   = ["Docker", "Kubernetes"]
  ci_cd        = ["GitLab CI", "GitHub Actions", "Jenkins"]
  observability = ["Grafana", "Prometheus"]
  coding       = ["Python", "Bash"]
  databases    = ["Redis", "InfluxDB", "SQL"]
}

# Recent work

resource "projects" "highlights" {
  project {
    title   = "Enterprise Cost Optimization"
    impact  = "Reduced cloud spend by 35% for a Fortune 500 company"
    details = "Implemented FinOps practices, right-sized resources, and optimized reserved instance strategy"
  }
  
  project {
    title   = "Multi-Region Infrastructure"
    impact  = "Designed resilient architecture spanning 3 regions with 99.99% uptime"
    details = "Created modular Terraform deployment with automated failover and disaster recovery"
  }
  
  project {
    title   = "DevOps Transformation"
    impact  = "Accelerated deployment frequency from monthly to daily releases"
    details = "Implemented GitLab CI pipelines with infrastructure validation gates"
  }
}

# Get in touch

resource "contact" "professional" {
  for_inquiries = "Consulting engagements, architecture reviews, cost optimization"
  email       = "your.email@example.com"
  linkedin    = "linkedin.com/in/yourprofile"
  twitter     = "twitter.com/yourhandle"
}
```

> "I build cloud infrastructure that works like it should: efficiently, reliably, and without surprise bills at the end of the month."

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=dark&hide_border=true)
