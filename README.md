# 한국어 대화 데이터 3D 시각화

7,400+ 개의 한국어 AI 대화 데이터를 3D 공간에서 시각화한 인터랙티브 프로젝트입니다.

## 🌟 특징

- **3D 시각화**: Three.js를 사용한 구형 데이터 배치
- **6개 클러스터**: 대화 데이터가 6개 그룹으로 분류
- **인터랙티브**: 마우스로 회전, 줌, 호버 시 상세 정보 표시
- **실시간 필터링**: 클러스터별 필터링 기능
- **Radial Gradient**: 중심에서 외곽으로 부드러운 그라데이션 효과

## 🚀 실행 방법

### 온라인
GitHub Pages에서 바로 확인: [https://yesochoi.github.io/ai-viz/](https://yesochoi.github.io/ai-viz/)

### 로컬
```bash
# 저장소 클론
git clone https://github.com/YesoChoi/ai-viz.git
cd ai-viz

# 로컬 서버 실행 (Python)
python3 -m http.server 8000

# 또는 Node.js
npx http-server -p 8000
```

브라우저에서 `http://localhost:8000` 접속

## 📊 데이터 구조

- **user_text**: 사용자 질문 텍스트
- **cluster_lv1**: 상위 클러스터 (0-18)
- **cluster_lv2**: 하위 클러스터 (0-5)
- **model**: 사용된 AI 모델 (gpt-3.5-turbo, gpt-4 등)

## 🎮 조작법

- 🖱️ **좌클릭 드래그**: 3D 회전
- 🖱️ **휠**: 줌 인/아웃
- 👆 **호버**: 데이터 포인트 상세 정보 보기
- 🔘 **클러스터 버튼**: 특정 클러스터만 필터링

## 🛠️ 기술 스택

- Three.js (3D 렌더링)
- PapaParse (CSV 파싱)
- Vanilla JavaScript
- HTML5 Canvas (그라데이션 텍스처)

## 📝 라이선스

MIT License

