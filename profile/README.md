# 🏃‍♂️ 모두의핏 (Fit4All) | NEXUSCORE

> **"모두를 위한 운동, 모두의핏"**
> 모든 사람을 위한 체육시설 예약 및 맞춤형 운동 프로그램을 제공하는 종합 스포츠 서비스 플랫폼입니다.

[![Landing Page](https://img.shields.io/badge/Website-Live_Now-4C6EF5?logo=airplay)](https://all4fit.co.kr) 
[![Play Store](https://img.shields.io/badge/Google_Play-Get_it_on-green?logo=googleplay)](https://play.google.com/store/apps/details?id=com.fitforeveryone.app&pcampaignid=web_share)
[![App Store](https://img.shields.io/badge/App_Store-Download-blue?logo=apple)](https://apps.apple.com/kr/app/%EB%AA%A8%EB%91%90%EC%9D%98-%ED%95%8F/id6754742148)
[![Figma](https://img.shields.io/badge/Figma-Design_System-F24E1E?logo=figma)](https://www.figma.com/design/eyFKN28IKXV25Y28znWMal/%EB%AA%A8%EB%91%90%EC%9D%98%ED%95%8F---%EC%9E%91%0A%EC%97%85-%EC%A7%84%ED%96%89?node-id=106-718)

---

## 📱 프로젝트 통합 개요

**모두의핏**은 NEXUSCORE가 총괄 기획하고 CLAPON과 협력하여 개발한 온-오프라인 통합 스포츠 플랫폼입니다. AWS EC2 기반의 **랜딩 페이지**와 Flutter/Supabase/Firebase 기반의 **고성능 모바일 앱**을 통해 사용자에게 끊김 없는 예약 경험을 제공합니다.

* **Project Lead**: NEXUSCORE (기획, 전략, 총괄 운영)
* **Development Partner**: CLAPON (서비스 개발 및 인프라 구축 협력)
* **Platform**: Web (Landing), iOS & Android (App)


---

## 👥 Meet the Team (NEXUSCORE)

본 프로젝트의 기획 및 PM을 담당한 핵심 인력입니다.

| **Lead PM / Strategy** | **Product Manager / Design** |
| :---: | :---: |
| <p align="center"><img src="https://avatars.githubusercontent.com/jinseok19" width="100" height="100" style="border-radius: 5%;"></p><p align="center"><a href="https://github.com/jinseok19"><img src="https://img.shields.io/badge/jinseok19-181717?style=for-the-social&logo=github&logoColor=white"/></a></p> | <p align="center"><img src="https://avatars.githubusercontent.com/hwruchan" width="100" height="100" style="border-radius: 5%;"></p><p align="center"><a href="https://github.com/hwruchan"><img src="https://img.shields.io/badge/hwruchan-181717?style=for-the-social&logo=github&logoColor=white"/></a></p> |
| **김진석 (Kim Jin-seok)** | **김정찬 (Kim Jeong-chan)** |
| 프로젝트 총괄 및 전략 기획 | 서비스 기획 및 UI/UX 설계 |

---

## 🎨 Service Journey: 기획에서 서비스까지

아이디어 구상부터 최종 배포까지, 프로젝트가 완성되는 전 과정을 시각화했습니다.

| **1. 화면 기획서** | **2. 디자인 시스템** | **3. 랜딩 페이지** | **4. 앱 화면** |
| :---: | :---: | :---: | :---: |
| <img src="images/readme/wireframe.png" width="200" alt="Wireframe"> | <img src="images/readme/design-system.png" width="200" alt="Design System"> | <img src="images/readme/web-preview.jpeg" width="200" alt="Landing Page"> | <img src="images/readme/app-combined.png" width="200" alt="App Screen"> |
| *UX 흐름 및 와이어프레임* | *Figma 디자인 시스템* | *[all4fit.co.kr](https://all4fit.co.kr)* | *iOS/Android 실서비스* |



---

## ✨ 핵심 서비스

### 1. 모바일 앱 (iOS / Android)
* **Cross-platform**: Flutter를 통한 일관된 사용자 경험 제공
* **실시간 알림**: Firebase(FCM)를 활용한 예약 및 활동 푸시 알림 구현
* **데이터 인프라**: Supabase 기반의 고속 데이터 연동 및 인증 시스템
* **스마트 예약**: 위치 기반 체육시설 실시간 조회 및 즉시 예약 시스템

### 2. 웹 플랫폼 (Landing & Admin)
* **안정적 배포**: AWS EC2 인프라 및 Nginx Reverse Proxy 환경 구축
* **정보 제공**: 서비스 제휴 체육시설 리스트 및 플랫폼 가치 전달
* **최적화**: Vanilla JS 기반의 가볍고 빠른 응답 속도 구현

---

## 🛠️ 기술 스택

### **Mobile & Backend**
* **Framework**: Flutter (Dart)
* **Backend/Database**: Supabase (PostgreSQL, Auth, Storage)
* **Push Service**: Firebase (Cloud Messaging)

### **Web & Infra**
* **Landing**: Vanilla JS, HTML5, CSS3
* **Server**: AWS EC2 (Ubuntu), Nginx
* **Process Management**: PM2

### **Design**
* **Tool**: Figma ([Design System](https://www.figma.com/design/eyFKN28IKXV25Y28znWMal/%EB%AA%A8%EB%91%90%0A%EC%9D%98%ED%95%8F---%EC%9E%91%EC%97%85-%EC%A7%84%ED%96%89?node-id=106-718))

---

## 🤝 파트너십 및 문의
* **Project Lead**: **NEXUSCORE** (넥서스코어)
* **Development Partner**: **CLAPON** (클랩온)
* **Official Email**: [nexuscore@nexuscore.co.kr](mailto:nexuscore@nexuscore.co.kr)
* **Download**: [App Store](https://apps.apple.com/kr/app/%EB%AA%A8%EB%91%90%EC%9D%98-%ED%95%8F/id6754742148) | [Play Store](https://play.google.com/store/apps/details?id=com.fitforeveryone.app&pcampaignid=web_share)

---
**Made with ❤️ by NEXUSCORE & CLAPON**
