# healthcare

# YourHealth AI 🏥🤖

AI-powered smart health assistant with symptom analysis, hospital locator, medicine recommendations, health reminders, and real-time navigation support.

---

# 🚀 Features

## 🩺 Symptom Checker

* AI-based symptom analysis
* Severity classification:

  * Mild
  * Moderate
  * Severe
* Recommended care suggestions

## 📍 Real-Time Location & Hospital Finder

* Detects user location using Geolocation API
* Interactive map using Leaflet.js
* Nearby hospital discovery using OpenStreetMap + Overpass API
* Route navigation to hospitals

## 💊 Medicine Recommendations

* Suggested medicines based on symptoms
* Dosage recommendations
* Timing and duration guidance
* PDF medicine schedule generation

## 🥗 Diet & Nutrition Guidance

* Recommended meals
* Foods to avoid
* Hydration suggestions

## 📂 Health Report Upload

* Upload PDF and image medical reports
* Local storage-based file management

## ⏰ Medication Reminders

* Add medicine reminders
* Weekly repeat scheduling
* Reminder management

## 🚨 Emergency SOS

* One-click emergency calling support

---

# 🛠️ Tech Stack

## Frontend

* HTML5
* Tailwind CSS
* JavaScript

## Maps & Navigation

* Leaflet.js
* Leaflet Routing Machine
* OpenStreetMap
* Overpass API
* OSRM Routing API

## PDF Generation

* jsPDF

## Storage

* Browser LocalStorage

---

# 🏗️ System Architecture

```text
User
  │
  ▼
Frontend UI (HTML + Tailwind + JS)
  │
  ├── Geolocation API
  ├── OpenStreetMap API
  ├── Overpass API
  ├── OSRM Routing API
  ├── LocalStorage
  └── jsPDF
```

---

# 📦 Project Structure

```bash
YourHealthAI/
│
├── index.html
├── assets/
│   ├── images/
│   └── icons/
│
├── README.md
```

---

# ⚙️ Installation & Setup

## 1. Clone Repository

```bash
git clone https://github.com/your-username/YourHealthAI.git
```

---

## 2. Navigate to Project

```bash
cd YourHealthAI
```

---

## 3. Run Locally

Simply open:

```bash
index.html
```

or use Live Server in VS Code.

---


# 🐳 Docker Setup

## Create Dockerfile

```dockerfile
FROM nginx:alpine

COPY . /usr/share/nginx/html

EXPOSE 80
```

---

## Build Docker Image

```bash
docker build -t yourhealthai .
```

---

## Run Container

```bash
docker run -d -p 80:80 yourhealthai
```

---

# ☸️ Kubernetes Deployment

## Deployment YAML

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: yourhealthai
spec:
  replicas: 2
  selector:
    matchLabels:
      app: yourhealthai
  template:
    metadata:
      labels:
        app: yourhealthai
    spec:
      containers:
      - name: yourhealthai
        image: yourhealthai:latest
        ports:
        - containerPort: 80
```

---

## Service YAML

```yaml
apiVersion: v1
kind: Service
metadata:
  name: yourhealthai-service
spec:
  type: NodePort
  selector:
    app: yourhealthai
  ports:
    - port: 80
      targetPort: 80
      nodePort: 30080
```

---

# 🔄 CI/CD Workflow

```text
GitHub Push
     ↓
Jenkins Pipeline
     ↓
Docker Image Build
     ↓
Push to Docker Hub
     ↓
Deploy to Kubernetes / EC2
```

---

# 📊 Monitoring Stack

* Prometheus
* Grafana
* CloudWatch

Metrics monitored:

* CPU usage
* Memory usage
* Application uptime
* Request rate

---

# 🔐 Security Features

* IAM least-privilege access
* Secure API requests
* Browser permission handling
* Restricted ingress access
* Docker container isolation

---

# 📸 Application Modules

## Dashboard

* Health assistant homepage
* User location display

## Hospital Navigation

* Nearby hospital markers
* Real-time routing

## AI Diagnosis

* Symptom-based diagnosis engine

## Report Management

* Upload and manage reports

## Reminder System

* Medicine scheduling and reminders

---

# 🌍 APIs Used

| API             | Purpose          |
| --------------- | ---------------- |
| OpenStreetMap   | Maps             |
| Overpass API    | Nearby hospitals |
| OSRM API        | Route navigation |
| Geolocation API | User location    |

---

# 📈 Future Improvements

* AI/ML symptom prediction
* User authentication
* Cloud database integration
* Push notifications
* Voice assistant
* Appointment booking
* Doctor consultation integration
* Mobile app version

---

# 👨‍💻 Author

THATIKANTI SIDDHARTHA

* DevOps Engineer
* Cloud & Infrastructure Automation
* Kubernetes | Docker | AWS | Terraform

GitHub:
`github.com/siddharth-thatikanti`

LinkedIn:
`linkedin.com/in/siddhartha-thatikanti-44a266367`

---

# 📄 License

This project is licensed under the MIT License.

---

# ⭐ Key Learning Outcomes

* Docker containerization
* Kubernetes deployments
* CI/CD automation
* Monitoring & observability
* API integration
* Real-time geolocation systems
* Infrastructure automation
* Frontend deployment architecture

Based on the uploaded project source code. 
