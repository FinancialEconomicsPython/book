# GitHub Pages 설정 파일 패키지

## 📦 포함된 파일들

이 패키지에는 Jupyter Book 기반 GitHub Pages를 구축하는데 필요한 모든 파일이 포함되어 있습니다.

### 파일 구조

```
jupyter-book-setup/
├── _config.yml              # Jupyter Book 기본 설정
├── _toc.yml                 # 사이트 목차 구조
├── intro.md                 # 홈페이지 (메인 페이지)
├── setup.md                 # 설치 및 사용법 페이지
├── license.md               # 라이선스 및 인용 페이지
├── requirements.txt         # Python 패키지 목록
├── references.bib           # 참고문헌 (향후 확장용)
├── SETUP_GUIDE.md          # ⭐ 자세한 설정 가이드
│
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Actions 자동 배포
│
├── chapters/
│   └── README.md            # 교재 코드 섹션 소개
│
├── readings/
│   └── README.md            # 추가 읽을거리 섹션 소개
│
└── appendix_online/
    └── README.md            # 온라인 부록 섹션 소개
```

---

## 🚀 빠른 시작 (3단계)

### 1단계: 파일 업로드

이 폴더의 모든 파일을 GitHub 저장소 (`FinancialEconomicsPython/book`)의 **루트 디렉토리**에 업로드하세요.

**주의사항:**
- 기존 `chapters/`, `readings/`, `appendix_online/` 폴더는 유지하세요
- 각 폴더에 `README.md`만 추가하면 됩니다
- 기존 README.md는 유지하거나 intro.md로 대체할 수 있습니다

### 2단계: GitHub Pages 활성화

1. GitHub 저장소 페이지 → **Settings** → **Pages**
2. **Source**에서 `GitHub Actions` 선택
3. 저장

### 3단계: 배포 확인

1. main 브랜치에 커밋 & 푸시
2. **Actions** 탭에서 빌드 진행 상황 확인
3. 완료 후 다음 주소에서 확인:
   - `https://financialeconomicspython.github.io/book/`

---

## 📋 상세 설정 가이드

자세한 설명은 `SETUP_GUIDE.md` 파일을 참고하세요.

주요 내용:
- GitHub Pages 설정 방법
- 커스터마이징 옵션
- 문제 해결 방법
- 업데이트 방법

---

## ✨ 주요 기능

### 자동 배포
- main 브랜치에 푸시하면 자동으로 사이트 업데이트
- GitHub Actions가 빌드 및 배포 자동 처리

### 깔끔한 네비게이션
- 좌측 사이드바: 전체 목차
- 우측 사이드바: 현재 페이지 목차
- 검색 기능

### 모바일 친화적
- 반응형 디자인
- 스마트폰에서도 편하게 읽기

### 다운로드 버튼
- 각 노트북에서 `.ipynb` 파일 다운로드 가능
- PDF 내보내기 기능

---

## 🎨 커스터마이징

### 로고 추가
1. 로고 이미지 파일을 저장소에 업로드 (예: `logo.png`)
2. `_config.yml`에서 수정:
```yaml
logo: logo.png
```

### 사이트 제목 변경
`_config.yml`에서:
```yaml
title: 원하는 제목
```

### 목차 순서 변경
`_toc.yml` 파일 수정

---

## 📝 기존 README.md 처리

두 가지 옵션이 있습니다:

### 옵션 1: 기존 README 유지 (권장)
- 기존 `README.md`를 그대로 두고
- `intro.md`를 홈페이지로 사용
- GitHub 저장소 페이지에서는 기존 README가 보임
- GitHub Pages에서는 intro.md가 홈페이지로 표시됨

### 옵션 2: README를 intro로 통합
- 기존 `README.md`의 내용을 `intro.md`에 통합
- 또는 `intro.md`를 `README.md`로 이름 변경하고 `_toc.yml` 수정

---

## 🔧 문제 해결

### 빌드가 실패하는 경우
1. **Actions** 탭에서 에러 로그 확인
2. `.yml` 파일의 들여쓰기 확인 (공백 2칸)
3. 파일 경로가 올바른지 확인

### 페이지가 업데이트되지 않는 경우
1. GitHub Actions 완료 대기 (5-10분 소요)
2. 브라우저 캐시 삭제 후 새로고침
3. 시크릿 브라우징 모드에서 확인

### 한글이 깨지는 경우
`_config.yml`에 다음이 포함되어 있는지 확인:
```yaml
sphinx:
  config:
    language: ko
```

---

## 📧 지원

설정 과정에서 문제가 발생하면:
- 📧 이메일: financialeconomicspython@gmail.com
- 📖 Jupyter Book 문서: https://jupyterbook.org/

---

## 🎯 다음 단계

1. ✅ 파일 업로드 완료
2. ✅ GitHub Pages 활성화
3. ✅ 첫 배포 확인
4. 📝 내용 추가 및 커스터마이징
5. 🎨 로고 및 스타일 개선
6. 📢 사용자에게 새 URL 공유

---

**성공적인 배포를 기원합니다! 🎉**
