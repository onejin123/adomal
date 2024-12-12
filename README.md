# 자취생들을 위한 냉장고 맞춤 레시피 웹 솔루션

> 간편한 재료 관리와 맞춤형 요리 추천으로 1인 가구의 생활을 더욱 효율적으로!

---

## 주요 기능

- **영수증 텍스트 추출**: 영수증 이미지를 업로드하여 구매한 재료 정보를 자동으로 입력.
- **냉장고 재료 관리**: 냉장고에 재료를 등록하고 유통기한을 관리.
- **맞춤형 요리 추천**: 냉장고에 있는 재료를 기반으로 레시피 추천.
- **요리 방법 및 이미지 제공**: GPT 및 DALL-E를 사용하여 요리 과정과 완성된 이미지 생성.
- **사용자 커뮤니티**: 다른 사용자의 레시피를 팔로우하고 좋아요로 소통.

---

## 기술 스택

### **Frontend**
- **React**: 사용자 인터페이스 구현.
- **TypeScript**: 안정적이고 확장 가능한 코드 작성.
- **SASS**: 스타일링.

### **Backend**
- **Node.js + Express**: RESTful API 서버 구축.
- **MongoDB**: 데이터 저장 및 관리.
- **JWT + Google OAuth**: 사용자 인증.

### **AI Integration**
- **Qwen OCR**: 영수증 텍스트 추출.
- **YOLOv5**: 냉장고 객체 탐지.
- **OpenAI GPT/DALL-E**: 요리 과정 및 이미지 생성.

### **Deployment**
- **AWS EC2**: AI 모델 배포 및 관리.
- **Vercel**: 프론트엔드 서버리스 배포.
- **Cloudinary**: 이미지 최적화 및 저장.

---

## 프로젝트 구조
📂 src ├── 📂 backend │ ├── 📂 models # 데이터베이스 모델 │ ├── 📂 routes # API 라우트 │ └── app.js # Express 서버 설정 ├── 📂 frontend │ ├── 📂 components # React 컴포넌트 │ ├── 📂 pages # 주요 페이지 │ └── index.tsx # React 진입점 └── 📂 ai-models ├── qwen.py # Qwen OCR API ├── yolo.py # YOLOv5 객체 탐지 └── flask_app.py # Flask API 서버
