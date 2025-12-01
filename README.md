# 🪨📄✂️ Rock–Paper–Scissors Image Classification
### Image Classification using Convolutional Neural Network (CNN) & TensorFlow

Project ini merupakan implementasi fundamental machine learning untuk mengenali gesture tangan Batu (Rock), Kertas (Paper), dan Gunting (Scissors) menggunakan deep learning berbasis Convolutional Neural Network (CNN).

---

## Deskripsi Project

Project ini bertujuan untuk membangun model klasifikasi gambar yang dapat mengenali gesture tangan: rock, paper, dan scissors. Dataset yang digunakan berasal dari Dicoding Academy, yang berisi kumpulan gambar tangan dengan pose berbeda.Model dilatih menggunakan TensorFlow dan Keras, dilengkapi dengan image augmentation untuk meningkatkan performa generalisasi model.

---

## Dataset

Dataset yang digunakan adalah:
- Rock-Paper-Scissors Dataset
  
  Sumber: Dicoding Academy
  Link: https://github.com/dicodingacademy/assets/releases/download/release/rockpaperscissors.zip

---

## Methodology: SDLC (Waterfall Model)
1. Planning: Identifying key issues in the manual monitoring workflow.
2. Analysis: Mapping existing processes, conducting root cause analysis using Fishbone diagrams.
3. Design: Developing system architecture and user interface sketches.
4. Implementation: Building Streamlit dashboards with Python and integrating Random Forest models.
5. Testing & Evaluation: Conducting user testing, confusion matrix evaluation, and cross-validation.

---

## Analysis (Mapping existing processes)

- Proses Bisnis Existing Register Kontrak
  ![PBE1](Diagrams/PBE1.png)

- Proses Bisnis Existing Monitoring Kontrak

  ![PBE2](Diagrams/PBE2.png)

---

## System Features
- 🔹 **Predictive Classification** — Contract risk level: *High*, *Medium*, *Low* using Random Forest.  
- 🔹 **Dual-Model System** — Comparison between *rule-based* and *machine learning*-based classification.  
- 🔹 **Interactive Dashboard** — Contract filtering by vendor, type, and risk category.  
- 🔹 **Visualization & Reporting** — Charts and “Top 50 High-Priority Contracts” table.  
- 🔹 **Email Notification System** — Automatic alerts for expiring or high-risk contracts.  
- 🔹 **Google Sheets Integration** — For both input and output data management.

---

## Tools & Technologies

| Category | Tools |
|-----------|-------|
| Programming | Python, Streamlit |
| Machine Learning | Scikit-learn, Random Forest, SMOTE, RandomizedSearchCV |
| Data Handling | Pandas, NumPy, Google Sheets API |
| Model Deployment | Joblib, Streamlit Cloud |
| Visualization | Matplotlib, Seaborn |
| Communication & Notification | SMTP Email Integration |
| Design & Documentation | Lucidchart, Draw.io |
| Methodology | SDLC (Waterfall) |

---

## Design System Architecture & Diagrams
  
- Use Case Diagram
  
  ![UCD](Diagrams/UCD.png)
  
- Activity Diagram
  
  ![AD](Diagrams/AD.png)

- Sequence Diagram
  
  ![SD](Diagrams/SD.png)

  
---

## System Architecture Overview
**Core Components:**
1. **Data Input Module** – Connects to Google Sheets and retrieves contract datasets.  
2. **Preprocessing Module** – Performs label encoding, SMOTE balancing, and noise injection.  
3. **Classification Engine** – Executes both Rule-Based and Random Forest prediction models.  
4. **Visualization & Alert Module** – Displays results on Streamlit dashboard and sends email alerts.  
5. **Output Module** – Stores predictions and evaluation results back to Google Sheets.

---

## Results & Evaluation

| Model | Accuracy | F1 (Low) | F1 (Medium) | F1 (High) | Rule-Based Alignment |
|--------|-----------|-----------|--------------|------------|----------------------|
| Random Forest (Iteration 1) | 73.3% | 0.67 | 0.15 | 0.84 | 86.1% |
| Random Forest (Iteration 2) | 81.7% | 0.64 | 0.62 | 0.89 | 82.7% |
| Random Forest (Iteration 3) | 78.3% | 0.53 | 0.62 | 0.86 | 81.8% |
| Random Forest (Iteration 4) | 68.3% | 0.60 | 0.45 | 0.77 | **92.3%** |

- **Strong correlation (r = 0.71)** between contract value and priority classification.  
- Random Forest model demonstrated **reliable predictive accuracy** and consistent results across validation sets.  
- User evaluation confirmed **dashboard usability** and **relevance to operational workflow**.  

---

## Key Contributions
- Designed and implemented an **end-to-end predictive contract monitoring system** aligned with IT governance principles.  
- Demonstrated **integration of business rules and machine learning** for practical decision support.  
- Enhanced **visibility and control** over procurement contracts within Bank XYZ’s IT Division.  
- Provided **academic and operational insights** for digital transformation in contract management.  

---

## Documentation 
- https://drive.google.com/file/d/1GuAnPc116wLy8czlikL17pjkVPRrsnK3/view?usp=sharing
  
  ![UI 1](UI%20Streamlit/UI%201.png)
  ![UI 2](UI%20Streamlit/UI%202.png)
  ![UI 3](UI%20Streamlit/UI%203.png)
  ![UI 4](UI%20Streamlit/UI%204.png)
  ![UI 5](UI%20Streamlit/UI%205.png)

---

## Conclusion
This project successfully bridges **Business Analytics** and **System Analysis**, demonstrating how predictive analytics can be embedded into operational workflows through structured system design.  
The resulting dashboard offers a practical model for **data-driven decision support**, applicable to future IT governance, ERP monitoring, and procurement systems.

> _“Transforming business insights into actionable systems through analytics and design.”_

---

