---
title: "Terraform"
date: 2023-05-10T08:16:07+02:00
draft: false
author: Thomas Panzeri
---

* `git init` - initializes a new Git repository
* `git clone [url]` - clones a remote repository to your local machine
* `git status` - displays the current status of the repository
* `git add [file]` - adds a file to the staging area
* `git add .` - adds all modified files to the staging area
* `git commit -m "[message]"` - commits changes to the local repository with a descriptive message
* `git push` - pushes changes from the local repository to the remote repository
* `git pull` - pulls changes from the remote repository to the local repository

## Google Cloud Platform (GCP)

### Compute Engine

#### Instance

```terraform
resource "google_compute_instance" "example" {
  name         = "example-instance"
  machine_type = "n1-standard-1"
  zone         = "us-central1-a"

  boot_disk {
    initialize_params {
      image = "debian-cloud/debian-10"
    }
  }

  network_interface {
    network = "default"
    access_config {
    }
  }
}
```

### Cloud Storage

#### Bucket

```
resource "google_storage_bucket" "example" {
  name          = "example-bucket"
  location      = "US"
  storage_class = "STANDARD"
}
```

Cloud SQL
Instance

arduino

resource "google_sql_database_instance" "example" {
  name             = "example-instance"
  database_version = "POSTGRES_13"
  region           = "us-central1"
  settings {
    tier = "db-f1-micro"
  }
}

User

java

resource "google_sql_user" "example" {
  name     = "example-user"
  instance = google_sql_database_instance.example.name
  password = "example-password"
}

Networking
VPC Network

arduino

resource "google_compute_network" "example" {
  name                    = "example-network"
  auto_create_subnetworks = true
}

Firewall Rule

arduino

resource "google_compute_firewall" "example" {
  name    = "example-firewall"
  network = google_compute_network.example.name

  allow {
    protocol = "tcp"
    ports    = ["80", "443"]
  }

  source_ranges = ["0.0.0.0/0"]
}

Identity and Access Management (IAM)
Service Account

python

resource "google_service_account" "example" {
  account_id = "example-account"
  display_name = "Example Service Account"
}

resource "google_service_account_key" "example" {
  service_account_id = google_service_account.example.id
}

IAM Member

java

resource "google_project_iam_member" "example" {
  project = var.project_id
  role    = "roles/storage.objectViewer"
  member  = "user:example@example.com"
}

