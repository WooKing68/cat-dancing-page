# 웹 페이지 배포 가이드

## 🎯 가장 쉬운 방법: Vercel

### 단계 1: 빌드
```bash
cd Z:\bhairava\programs\_Book_Claude-Code-main\week1\Fri\cat-dancing-page
npm run build
```

### 단계 2: Vercel 설치 및 배포
```bash
# Vercel CLI 설치
npm install -g vercel

# 배포 (첫 실행시 브라우저에서 로그인)
vercel
```

### 단계 3: 완료!
- 배포 URL을 받습니다 (예: https://cat-dancing-xxxxx.vercel.app)
- 이 URL을 누구와도 공유할 수 있습니다!

---

## 🔄 업데이트 방법
코드를 수정한 후:
```bash
vercel --prod
```

---

## 📝 다른 옵션들

### Netlify (드래그 앤 드롭)
1. `npm run build` 실행
2. https://app.netlify.com 접속
3. `dist` 폴더를 드래그 앤 드롭
4. 완료!

### GitHub Pages
1. GitHub 저장소 생성
2. 코드 푸시
3. Settings → Pages에서 활성화

### Cloudflare Pages
1. https://pages.cloudflare.com 접속
2. GitHub 연동 또는 직접 업로드
3. 빌드 명령: `npm run build`
4. 출력 디렉터리: `dist`

---

## 💡 팁
- 모든 서비스 무료입니다!
- Vercel이 가장 빠르고 쉽습니다
- 코드 수정 후 다시 배포하면 자동 업데이트됩니다
- HTTPS가 자동으로 적용됩니다

---

## 🆘 문제 해결

### "command not found" 에러
```bash
# Node.js가 설치되어 있는지 확인
node --version
npm --version

# 없으면 https://nodejs.org 에서 설치
```

### 빌드 에러
```bash
# 의존성 재설치
npm install
npm run build
```
