# ☁️ Internship Task 3 – Multi-Cloud Architecture

## ✅ Objective
Design a multi-cloud architecture that demonstrates interaction between services hosted on **two different cloud platforms** – **Google Cloud Platform (GCP)** and **Amazon Web Services (AWS)**.

---

## 🧱 Architecture Overview

This task demonstrates interoperability between:
- **Google Cloud Storage (GCS)** – used to store a public `.txt` file.
- **AWS S3 Static Website** – used to host a simple webpage that links to and embeds the GCS file.

### 🔁 Inter-Cloud Communication
The webpage hosted on AWS directly accesses and displays the file stored on GCP via its public URL, simulating a cross-cloud integrated system.

---

## 🔨 Tools and Services Used

| Cloud | Service Used         | Purpose                        |
|-------|----------------------|--------------------------------|
| GCP   | Google Cloud Storage | Store a public `.txt` file     |
| AWS   | S3 Static Website    | Host an HTML page referencing GCS |

---

## 🌐 Public Resources

- 📄 **GCS Public File**:  
  [`cloud_computing.txt`](https://storage.googleapis.com/gcs-intern-bucket-2025/cloud_computing.txt)

- 🖥️ **S3 Hosted Website** (Replace with your actual endpoint):  
  `http://your-bucket-name.s3-website-<region>.amazonaws.com`

---

## 🗂️ Files Included in This Repo

```bash
task-3-multicloud/
├── index.html           # AWS S3 hosted webpage
├── screenshots/
│   ├── gcs_file.png     # GCS public file view
│   ├── s3_upload.png    # Uploading index.html to S3
│   └── s3_site.png      # Live S3 static site showing GCS file
└── README.md            # This documentation
