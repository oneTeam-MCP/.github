# 🏫 **SMUS: AI Agent(Custom MCP-driven)를 활용한 상명대학교 통합 정보 허브**
</br>

## 🟦 프로젝트 목적

본 과제는 질의응답 수준의 Chatbot을 넘어서 상명대학교라는 특정 도메인에 특화된 통합 정보 시스템을 구축하는 것을 목표로 합니다. 특히 MCP(Model Context Protocol) 기반의 Custom AI 에이전트를 활용하여 대화형 인터페이스 형태를 통해 학생들의 실제 업무 및 학습 활동을 효과적으로 지원하는 에이전틱 시스템을 구현하고자 합니다.

또한 개인 맞춤형 서비스 제공을 통해 각 학생의 학사 일정을 자동으로 추적하고 미제출 과제를 실시간으로 조회해주는 기능을 제공합니다. 또한 수강 과목, 시험 일정, 학사 공지사항 등을 통합적으로 관리하여 학생들이 학업 관련 정보를 한 곳에서 편리하게 확인하고 관리할 수 있도록 지원합니다. 이를 통해 학생들은 정보 검색에 소요되는 시간을 절감하고 중요한 학사 일정이나 과제 마감일을 놓치지 않으며 보다 효율적인 대학 생활을 할 수 있습니다.

궁극적으로 본 프로젝트는 AI 기술을 활용하여 대학 생활의 편의성을 극대화하고 학습 생산성을 향상시키는 실용적인 솔루션을 제공하는 것을 목적으로 합니다.

</br>

## 🟦 프로젝트 내용

**1. 시스템 아키텍처**
- Backend:
    - AWS EC2 인스턴스 내에 Spring 프레임워크 기반으로 구축된 MCP Host와 RESTful API 서버를 Docker 컨테이너로 배포했습니다.
    - Nginx 리버스 프록시와 Certbot을 통한 HTTPS 보안 통신을 적용하여 안전한 데이터 전송 환경을 구성했습니다.
    - GitHub Actions를 활용한 CI/CD 파이프라인을 구축했습니다.
- Frontend:
    - React 프레임워크와 TypeScript를 활용하여 SPA(Single Page Application) 형태의 애플리케이션 구축했습니다.
    - 학사 대시보드, Chatbot AI 인터페이스, 일정 관리 화면 등을 설계•구현하고, AJAX를 활용하여 MCP Host 및 Backend 서버와 통신했습니다.
    - Vercel을 통해 자동 배포 파이프라인을 구축했습니다.
    
**2. 데이터 수집**
- AWS Lambda와 API GATEWAY로 구현된 서버리스 크롤링 시스템입니다.
- 메타 데이터는 AWS RDS에, 파일(pdf, hwp)은 AWS S3에 저장합니다.
- AWS Lambda를 이용하여 개인화 데이터 및 학교 공용 데이터를 주기적으로 크롤링합니다.
    
**3. MCP 서버 개발**
- FastMCP 프레임워크를 활용하여 상명대학교 도메인에 특화된 MCP 서버를 개발했습니다.
- Tools 모듈에는 학사 일정 조회, 학교 공지사항 검색, 학식 메뉴 조회, 개인 일정 관리 등 학교생활에 필요한 기능들을 구현했습니다.
- Prompts 모듈에서는 날짜/시간 처리, 키워드 매칭 등 가이드라인을 제공하여 정확하고 일관된 응답을 제공할 수 있도록 했습니다.

**4. AI 에이전트 시스템 구현**
- GPT-4o 모델을 활용하여 자연어 처리 능력을 확보하고, Smithery를 통해 MCP 서버와 연결하는 MCP Host를 Spring AI로 구축했습니다.
- 사용자 질의가 입력되면 LLM이 FastMCP 서버와 통신하여 필요한 MCP Tool을 선택 및 사용하여 자연어로 응답을 구성했습니다.
- LangGraph를 활용하여 대화 맥락을 관리하고 스트리밍 응답 방식을 적용하여 사용자에게 실시간으로 응답을 제공했습니다.

</br>

## 🟦 Team

| 김재관 | 김정찬 | 김진석 | 맹의현 | 염다인 |
| --- | --- | --- | --- | --- |
| <p align="center"><img src="https://avatars.githubusercontent.com/KJaeKwan" width="100" height="100" style="border-radius: 5%;"></p><p align="center"><a href="https://github.com/KJaeKwan"><img src="https://img.shields.io/badge/KJaeKwan-181717?style=for-the-social&logo=github&logoColor=white"/></a></p> | <p align="center"><img src="https://avatars.githubusercontent.com/hwruchan" width="100" height="100" style="border-radius: 5%;"></p><p align="center"><a href="https://github.com/hwruchan"><img src="https://img.shields.io/badge/hwruchan-181717?style=for-the-social&logo=github&logoColor=white"/></a></p> | <p align="center"><img src="https://avatars.githubusercontent.com/jinseok19" width="100" height="100" style="border-radius: 5%;"></p><p align="center"><a href="https://github.com/jinseok19"><img src="https://img.shields.io/badge/jinseok19-181717?style=for-the-social&logo=github&logoColor=white"/></a></p> | <p align="center"><img src="https://avatars.githubusercontent.com/maeng00" width="100" height="100" style="border-radius: 5%;"></p><p align="center"><a href="https://github.com/maeng00"><img src="https://img.shields.io/badge/maeng00-181717?style=for-the-social&logo=github&logoColor=white"/></a></p> | <p align="center"><img src="https://avatars.githubusercontent.com/dainsla" width="100" height="100" style="border-radius: 5%;"></p><p align="center"><a href="https://github.com/dainsla"><img src="https://img.shields.io/badge/dainsla-181717?style=for-the-social&logo=github&logoColor=white"/></a></p> |
</br>

## 🟦 Architecture
<img width="2815" height="1254" alt="Image" src="https://github.com/user-attachments/assets/624c676e-5b5b-4502-9518-1eed73bbafad" />

</br>
</br>

## 🚀 Tech Stack

### 📌 Framework

<img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-social&logo=springboot&logoColor=white" />

### 📌 Build Tool

<img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-social&logo=Gradle&logoColor=white">

### 📌 Database

<img src="https://img.shields.io/badge/Spring Data JPA-6DB33F?style=for-the-social&logo=Databricks&logoColor=white"> <img src="https://img.shields.io/badge/RDS-527FFF?style=for-the-social&logo=amazonrds&logoColor=white"> <img src="https://img.shields.io/badge/Redis-%23DC382D.svg?style=for-the-social&logo=redis&logoColor=white" />

### 📌 Security

<img src="https://img.shields.io/badge/Spring Security-6DB33F?style=for-the-social&logo=springsecurity&logoColor=white">

### 📌 Cloud

<img src ="https://img.shields.io/badge/EC2-FF9900?style=for-the-social&logo=amazonec2&logoColor=white"> <img src ="https://img.shields.io/badge/S3-69A31?style=for-the-social&logo=amazons3&logoColor=white"> <img src="https://img.shields.io/badge/RDS-527FFF?style=for-the-social&logo=amazonrds&logoColor=white"> <img src="[https://img.shields.io/badge/CLOVA OCR-03C75A?style=flat](https://img.shields.io/badge/CLOVA%20OCR-03C75A?style=flat)">

### 📌 API Documentation

<img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-social&logo=swagger&logoColor=white">

### 📌 CI/CD

<img src="https://img.shields.io/badge/GitHub Actions-2088FF?style=for-the-social&logo=githubactions&logoColor=white"> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-social&logo=docker&logoColor=white"> 

### 📌 Team Collaboration

<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-social&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/Git-F05032?style=for-the-social&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-social&logo=notion&logoColor=white" /> <img src="https://img.shields.io/badge/Discord-%237289DA.svg?style=for-the-social&logo=discord&logoColor=white" /> <img src="https://img.shields.io/badge/Figma-%23F24E1E.svg?style=for-the-social&logo=figma&logoColor=white" />

</br>

<br>
