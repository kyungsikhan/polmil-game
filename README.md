# Pol-Mil Crisis Commander 2026: G4 Wargame (Web Deployment Package)

이 폴더(`dist/`)는 오픈 웹(GitHub Pages, Vercel, Netlify, Cloudflare Pages 등)에 즉시 배포할 수 있는 **순수 정적 웹 패키지**입니다.

## 📦 구성 요소
- `index.html`: 4개국 라운드 테이블, 텔레메트리, 시나리오 및 교차 작전 로그가 모두 통합된 메인 웹 애플리케이션 (v6.4)
- `assets/`: 4개국 국기(SVG/PNG) 및 4대 위기 시나리오 고화질 전술 배경 이미지

---

## 🚀 배포 방법 가이드

### 1. Netlify Drop (가장 쉬운 10초 배포 - 회원가입 후 드래그 앤 드롭)
1. [https://app.netlify.com/drop](https://app.netlify.com/drop) 접속
2. 현재 `dist` 폴더 전체를 브라우저 화면의 점선 영역으로 드래그 앤 드롭
3. 5초 후 자동으로 고유한 공개 웹 주소(`https://xxxx.netlify.app`) 생성 완료!

### 2. GitHub Pages (가장 권장하는 정석 배포 - 영구 무료 호스팅)
1. GitHub(https://github.com)에서 새 Repository 생성 (예: `polmil-wargame`)
2. `dist` 폴더 안에서 아래 명령어를 실행하여 푸시:
   ```bash
   cd dist
   git init
   git add .
   git commit -m "Deploy Pol-Mil Crisis Commander Arena"
   git branch -M main
   git remote add origin https://github.com/kyungsikhan/polmil-wargame.git
   git push -u origin main
   ```
3. GitHub 저장소의 **Settings -> Pages** 메뉴로 이동
4. **Branch**를 `main` / `/(root)`로 지정하고 **Save** 클릭
5. 1~2분 후 `https://kyungsikhan.github.io/polmil-wargame/` 주소로 전 세계 공개 배포 완료!

### 3. Vercel 배포
1. [https://vercel.com](https://vercel.com) 로그인
2. `Add New...` -> `Project` 선택 후 `dist` 폴더 업로드 또는 GitHub 저장소 연동
3. 클릭 한 번으로 `https://polmil-wargame.vercel.app` 형태의 배포 URL 생성
