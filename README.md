# CapitalXtend App

capitalxtend.com을 WebView로 래핑한 Android APK.

## APK 빌드 방법

### 1. GitHub에 올리기
```bash
git init
git add .
git commit -m "init"
git remote add origin https://github.com/<YOUR_USERNAME>/capitalxtend-app.git
git push -u origin main
```

### 2. GitHub Actions 빌드 확인
- GitHub 레포 → **Actions** 탭
- `Build APK` 워크플로 자동 실행
- 완료 후 **Artifacts** 에서 `capitalxtend-debug.apk` 다운로드

## 파일 구조
```
capitalxtend-app/
├── .github/workflows/build-apk.yml  # 자동 빌드
├── www/index.html                    # fallback
├── capacitor.config.json             # 앱 설정
└── package.json
```

## 앱 정보
- **앱 ID**: com.capitalxtend.app
- **타겟 URL**: https://capitalxtend.com
- **빌드**: Debug APK (테스트용)

> 릴리즈 APK (Play Store용)가 필요하면 keystore 서명 단계 추가 필요.
