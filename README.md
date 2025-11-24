# 🚀 Real-Time CRM Analytics Dashboard  
### AI + Data + Event-Driven CRM Analytics Platform

A modular, microservices-based CRM Analytics platform that ingests customer events in real-time, processes them using Apache Kafka, performs machine learning predictions, and visualizes insights through a modern React dashboard.

This project is designed with a production-style architecture often used in companies like Salesforce, AWS, and other major product-based organizations.

---

## 📊 Project Highlights
- ⚡ Event-driven microservices architecture  
- 🟩 Spring Boot ingestion service  
- 🟦 Kafka stream-processing service  
- 🤖 FastAPI ML scoring microservice  
- 📈 React-based analytics dashboard  
- 🐳 Full Docker Compose setup  
- 🔁 Automated CI/CD via GitHub Actions  
- ☸️ Kubernetes-ready manifests  
- 📡 Monitoring placeholder (Prometheus + Grafana)

---

## 🧱 Architecture Overview

```
[ Client ] 
    ↓ (REST)
[ Ingest Service ] → Kafka → [ Stream Processor ] → DB
                                         ↓
                                 [ ML Service ]
                                         ↓
                                   [ Dashboard ]
```

---

## 📁 Project Structure
```
crm-analytics/
│
├── ingest-service/           # Spring Boot REST API for event ingestion
├── stream-processor/         # Kafka Consumer for analytics
├── ml-service/               # FastAPI ML microservice
├── dashboard/                # React dashboard UI
│
├── scripts/                  # Sample data generators
├── k8s/                      # Kubernetes manifests
├── monitoring/               # Monitoring configurations
│
├── docker-compose.yml        # Dev stack orchestrator
├── .github/workflows/ci.yml  # CI/CD pipeline
└── README.md                 # Project documentation
```

---

## ⚙️ Tech Stack

### **Backend**
- Java 17  
- Spring Boot  
- Apache Kafka  
- PostgreSQL  

### **Machine Learning**
- Python  
- FastAPI  
- scikit-learn  
- XGBoost  

### **Frontend**
- React  
- Axios  
- Recharts  

### **DevOps / Cloud**
- Docker  
- Docker Compose  
- GitHub Actions  
- Kubernetes Manifests  

---

## ▶️ Running the Project Locally

Run the full stack with one command:

```bash
docker-compose up --build
```

---

## 📥 Sample Event API (Ingest Service)

**POST /api/v1/events/lead**

```json
{
  "lead_id": "L-1001",
  "name": "John Doe",
  "source": "web",
  "timestamp": "2025-11-24T10:00:00Z"
}
```

---

## 📊 Dashboard Features
- Real-time lead analytics  
- Lead conversion probability (ML powered)  
- Sales funnel insights  
- Opportunity metrics  
- Processing latency and event statistics  

---

## 🧪 Testing

### **Backend**
- JUnit (Spring Boot)  

### **ML Service**
- pytest  

### **Frontend**
- Jest + React Testing Library  

---

## 🚀 Deployment (Optional)

Deploy all services on Kubernetes:

```bash
kubectl apply -f k8s/
```

---

## 📌 Why This Project Is Valuable

This project demonstrates real-world software engineering skills:

- Scalable microservices  
- Real-time streaming pipelines  
- ML integration  
- Cloud-native architecture  
- Industry-standard DevOps practices  

Perfect for opportunities at:
- Salesforce  
- Amazon  
- Microsoft  
- Any product-based company  

---


