---

## 🚀 Featured Project: E-Commerce ETL Pipeline

<div align="center">

<a href="https://github.com/sarthakgaware2002/E-CommerceETLProject">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=sarthakgaware2002&repo=E-CommerceETLProject&theme=midnight-purple&hide_border=true&bg_color=0f0c29&title_color=00d4ff&icon_color=a78bfa&text_color=ffffff" />
</a>

</div>

<br/>

<p align="center">
<b>End-to-End Scalable ETL Pipeline using AWS, Spark, Hive & ClickHouse</b>
</p>

---

### 🏗️ Architecture Overview

<p align="center">
  <img src="https://raw.githubusercontent.com/sarthakgaware2002/E-CommerceETLProject/main/ProjectArchitecture.png" width="800"/>
</p>

---

### ⚙️ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/AWS%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS%20RDS-527FFF?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hive-FDEE21?style=for-the-badge&logo=apachehive&logoColor=black"/>
  <img src="https://img.shields.io/badge/ClickHouse-FFCC01?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
</p>

---

### 🔄 Pipeline Flow

```text
RDS (Structured Data)
        │
        ▼
   Apache Spark (EMR)
        │
        ▼
MongoDB → Pandas → S3 (L1)
        │
        ▼
   Data Transformation (Spark)
        │
        ▼
   Hive (SCD Layer)
        │
        ▼
   S3 (L2 - Processed Data)
        │
        ▼
   ClickHouse (Analytics)
