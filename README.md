provider "github" {
  alias = "profile"
}

locals {
  name       = "Marin Govedarski"
  experience = "8+ years"
  interests  = [
    "Cloud Cost Optimization Strategies & FinOps",
    "Infrastructure Automation at Scale",
    "Platform Engineering",
    "DevSecOps Practices",
    "Technical Pre-Sales Architecture"
  ]
  learning   = [
    "Advanced FinOps Principles",
    "AI Integration in Infrastructure",
    "Multi-Cloud Governance"
  ]
  collaboration = [
    "Open Source Infrastructure Tools",
    "Cloud Architecture Consulting",
    "Technical Content Creation"
  ]
  certifications = [
    "Certified SAFe DevOps Practitioner"
  ]
}

resource "github_profile" "identity" {
  name        = local.name
  role        = "Cloud Solutions Architect | FinOps Specialist | SRE/DevOps"
  status      = "Currently contracting as a Solutions Architect"
  experience  = local.experience
  focus       = "Cloud Architecture, Cost Optimization, Pre-Sales Solutions"
  quote       = "Infrastructure as code isn't just about automation; it's about creating a predictable path to success."
}

# Tech Stack

module "cloud_platforms" {
  source = "./expertise"
  
  gcp = {
    level       = "Expert"
    years       = 5
    specialties = ["Architecture", "Cost Optimization", "Infrastructure Design"]
  }
  
  aws = {
    level       = "Advanced"
    years       = 3
    specialties = ["Solutions Architecture", "Cloud-Native Services"]
  }
}

resource "platform_expertise" "spacelift" {
  level              = "Specialist"
  implementation     = true
  optimization       = true
  governance         = true
  policy_as_code     = true
  stack_management   = true
}

resource "iac_toolkit" "primary" {
  terraform = {
    level         = "Expert"
    specialties   = ["Module Design", "State Management", "Multi-environment"]
    version_range = "1.0.0-1.5.7"
  }
  
  opentofu = {
    level       = "Expert"
    specialties = ["Migration from Terraform", "Custom Providers"]
  }
  
  ansible = {
    level       = "Advanced"
    specialties = ["Role Development", "Configuration Management"]
  }
}

resource "technical_skillset" "devops" {
  ci_cd = {
    gitlab_ci = {
      level       = "Expert"
      specialties = ["Pipeline Optimization", "Multi-stage Deployments"]
    }
    github_actions = {
      level       = "Advanced"
      specialties = ["Workflow Automation", "Matrix Builds"]
    }
    jenkins = {
      level       = "Advanced" 
      specialties = ["Pipeline as Code", "Job Management"]
    }
  }
  
  observability = {
    grafana = {
      level       = "Advanced"
      specialties = ["Dashboard Design", "Alerting"]
    }
    prometheus = {
      level       = "Advanced"
      specialties = ["Query Optimization", "Alert Rules"]
    }
  }
  
  containers = {
    docker = {
      level       = "Expert"
      specialties = ["Image Optimization", "Multi-stage Builds"]
    }
    kubernetes = {
      level       = "Expert"
      specialties = ["Cluster Management", "Resource Optimization", "RBAC"]
    }
  }
  
  version_control = {
    git = {
      level       = "Expert"
      specialties = ["Github", "Gitlab", "Bitbucket"]
    }
  }
}

resource "development_skills" "languages" {
  primary = {
    python = {
      level       = "Intermidiate"
      specialties = ["Automation Scripts", "Data Processing", "API Development"]
    }
    bash = {
      level       = "Advanced"
      specialties = ["System Automation", "Deployment Scripts"]
    }
  }
  
  secondary = {
    powershell = {
      level       = "Expert"
      specialties = ["Windows Automation", "Azure Management"]
    }
    groovy = {
      level       = "Intermidiate"
      specialties = ["Jenkins Pipelines", "Build Scripts"]
    }
  }
}

resource "data_management" "databases" {
  nosql = {
    redis = {
      level       = "Advanced"
      specialties = ["Caching Strategies", "Performance Tuning"]
    }
    influxdb = {
      level       = "Advanced"
      specialties = ["Time Series Data", "Monitoring Integration"]
    }
  }
  
  sql = {
    level       = "Intermediate"
    specialties = ["Query Optimization", "Schema Design"]
  }
}

resource "system_administration" "platforms" {
  linux = {
    level       = "Expert"
    specialties = ["Performance Tuning", "Security Hardening", "Automation"]
  }
  
  windows = {
    level       = "Advanced"
    specialties = ["Server Management", "PowerShell Automation"]
  }
}

resource "network_services" "edge" {
  cloudflare = {
    level       = "Advanced"
    specialties = ["DNS Management", "CDN Configuration", "WAF Policies"]
  }
}

resource "contact_methods" "professional" {
  linkedin = "https://www.linkedin.com/in/mgd-01b439163/"
  twitter  = "https://twitter.com/yourhandle"
}

output "focus_areas" {
  description = "Current professional focus areas"
  value = {
    cloud_cost_optimization = {
      techniques = [
        "Right-sizing Resources",
        "Reserved Instance Planning",
        "Spot Instance Strategies",
        "FinOps Implementation"
      ]
    }
    
    architecture_design = {
      specialties = [
        "Microservices",
        "Serverless Architecture",
        "Multi-region Deployments",
        "Disaster Recovery"
      ]
    }
    
    pre_sales = {
      strengths = [
        "Technical Solution Design",
        "Client Requirement Analysis",
        "Cost-Benefit Optimization",
        "Architecture Presentations"
      ]
    }
  }
}

# GitHub stats visual element - uncomment and replace username
# ![GitHub Stats](https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=dark)
