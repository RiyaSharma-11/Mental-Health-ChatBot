## 🔄 Tech Stack Workflow & Data Flow

The Mental Health Chatbot follows a structured pipeline architecture where user input is processed through multiple layers including frontend, backend, AI models, screening, and response generation.
---

### 🟢 1. User Interaction (Frontend)
- Web Interface: React  
- Mobile Interface: Flutter  
- Communication: WebSocket / Firebase  

➡️ Users send messages like *"I feel anxious"*

---

### 🔵 2. Backend Processing
- Frameworks: FastAPI / Django / Node.js  
- Handles API requests (`/chat`)  
- Performs:
  - Input validation  
  - User authentication (JWT/OAuth2)  
  - Anonymous access support  

---

### 🧠 3. AI/NLP Processing
- Models: DistilBERT / IndicBERT  
- Functions:
  - Intent detection  
  - Sentiment analysis  
  - Severity classification  

---

### 📊 4. Screening Engine
- Uses: PHQ-9 / GAD-7  
- Outputs:
  - Mental health score  
  - Risk level (mild / moderate / severe)  

---

### 📚 5. Recommendation Engine
- Tools: FAISS / pgvector  
- Provides:
  - Self-help resources  
  - Videos & audio  
  - Coping strategies  

---

### 🗄 6. Data Storage
- PostgreSQL → User profiles & screening scores  
- MongoDB → Chat history  
- AWS S3 / MinIO → Media files  

---

### 🔁 7. Response Generation
- Combines:
  - AI results  
  - Screening outcomes  
  - Recommended resources  
- Sends structured JSON response  

---

### 🖥 8. Frontend Display
- Displays:
  - Chat responses  
  - Suggestions  
  - Emergency support (if needed)  

---

### ☁️ 9. Deployment
- Deployed using **Streamlit Cloud**  
- Accessible via web browser  
- Real-time interaction enabled  

---

### 🔐 Security & Monitoring
- TLS/SSL Encryption  
- AES-256 Data Protection  
- JWT/OAuth2 Authentication  
- Monitoring via dashboards  

---

### 📌 Summary
This system ensures smooth data flow from user input to intelligent response generation, enabling real-time mental health support with secure and scalable architecture.
