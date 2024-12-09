![header](https://capsule-render.vercel.app/api?type=waving&color=A9DFBF&text=MSA%20Study&fontColor=008000&alignment-baseline="middle"&fontAlign=50&fontAlignY=50&height=150&desc=딥다이브%20백엔드%20MSA%20스터디&descAlign=50&descAlignY=80&)

<div align="center">

  ### 💻 What We Make 💻

  간단한 블로그 플랫폼을 마이크로서비스 아키텍처(MSA)를 사용하여 구축.  
  Spring Boot 기반의 각 서비스는 MSA에서 필요한 다양한 기능을 Spring Cloud를 활용해 처리합니다.  

  </br>

  ### 📚 Tech Stack 📚
  
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=Java&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=Spring&logoColor=white">
  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=SpringBoot&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white">
  <br>
  <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=RabbitMQ&logoColor=white">
  <img src="https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=ApacheKafka&logoColor=white">
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white">
  <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=Grafana&logoColor=white">

  <br/><br/>

  ### 🛠 Tools 🛠
  
  <img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white">
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">

  </br>

</div>

---

## **참고 사항**

### **다양한 구현 및 구성 가능성**
이 프로젝트는 여러 사람이 각자의 프로젝트를 진행하는 스터디의 일환으로 설계되었습니다.  
따라서 각 팀원은 자신만의 프로젝트 환경에 맞게 구현 및 구성을 조정했습니다.  

### **공통 목표**
- 각 참여자는 **MSA 설계 및 구현에 대한 이해**를 목적으로 하며, 서비스 간 독립성과 통합을 고려한 설계를 학습합니다.
- 프로젝트의 결과물은 스터디 공유와 피드백을 통해 지속적으로 발전될 수 있습니다.

### **각자의 프로젝트 별 다양성**
- 일부 팀원은 Kafka 대신 RabbitMQ만 사용하거나, MySQL 대신 NoSQL을 사용하는 등 개별적인 구성이 가능합니다.
- 세부적인 인증/인가 방법(JWT, OAuth 등)도 참여자별로 다를 수 있습니다.
- 도커를 이용한 배포도 추가될 수 있습니다.

---

## **1. 프로젝트 개요**

### **주제**
간단한 [블로그 모놀리식 프로젝트](https://github.com/deepdive-msa-study/blog-server)를 각자의 방법으로 MSA로 마이그레이션  
Spring Boot 기반으로 각 서비스를 개발하며, Spring Cloud를 사용해 서비스 간 통신, 구성 관리, 모니터링 등을 구현.


---

## **2. 목표**

- **MSA 설계 및 구현 과정 학습**:
    - 서비스 간 독립성 및 데이터 경계 유지
- **중앙화된 설정 관리 학습**:
    - Spring Cloud Config와 RabbitMQ를 통한 재배포 없는 설정 반영 환경 구현
- **장애 대응 및 모니터링 학습**:
    - Prometheus와 Grafana를 활용한 모니터링 및 시각화

---

## **3. 서비스 구성**

### **1) 비즈니스 서비스**
- **User Service**: 사용자 관리 및 인증/인가
- **Post Service**: 게시글 작성 및 관리
- **Comment Service**: 댓글 작성 및 관리
- **Hashtag Service**: 검색을 위한 해시태그

### **2) 마이크로서비스 기술 스택**
- **Spring Boot**: 각 서비스 구현
- **Spring Cloud**: Eureka, Config Server, API Gateway, Spring Cloud Bus 활용
- **RabbitMQ**: 이벤트 기반 통신
- **Kafka**: 데이터 변경 사항 전달 및 비동기 통신
- **Zipkin**: 분산 추적
- **Prometheus & Grafana**: 모니터링 및 시각화

---
