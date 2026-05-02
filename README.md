# ⚡ Pikachu Hologram AR

피카츄 카드를 비추면 홀로그램 피카츄가 나오는 AR 데모.
THUNDER PUNCH 버튼 누르면 펀치 애니메이션 + 8방향 번개 발사 ⚡

## 🚀 GitHub Pages 배포 (3분 컷)

### 1. GitHub에서 새 repo 생성
- https://github.com/new
- Repository name: `pikachu-ar` (또는 원하는 이름)
- **Public** 으로 설정 (Pages는 Public 무료)
- "Create repository" 클릭

### 2. 파일 업로드
이 폴더의 **모든 파일**을 새 repo에 업로드:
- 새 repo 페이지에서 "uploading an existing file" 클릭
- 폴더 통째로 드래그 (`index.html` + `assets/` 폴더 같이)
- "Commit changes" 클릭

### 3. Pages 활성화
- 그 repo의 **Settings** 탭 클릭
- 왼쪽 메뉴 **Pages** 클릭
- **Source**: `Deploy from a branch`
- **Branch**: `main` / `(root)` 선택
- **Save** 클릭
- 1~2분 후 상단에 URL 표시됨: `https://본인이름.github.io/pikachu-ar/`

### 4. 폰으로 접속
- 위 URL을 폰 브라우저로 열기
- ⚡ SUMMON ⚡ 버튼 누르고 카메라 권한 허용
- Pikachu 카드(인쇄 또는 다른 화면)를 비추면 등장!
- THUNDER PUNCH 버튼으로 공격 ⚡

---

## 📦 파일 구조
```
pikachu-ar/
├── index.html              ← 메인 앱
└── assets/
    ├── Combo_Punch.fbx     ← 피카츄 모델 + 펀치 애니메이션
    ├── pikachu_card.mind   ← AR 카드 트래킹 데이터 (이미 컴파일됨!)
    └── pikachu_card.jpg    ← 참고용 카드 이미지
```

## ⚡ 작동 방식
- **MindAR.js**: 카드 이미지 인식
- **Three.js**: 3D 렌더링 + 커스텀 GLSL 셰이더
- **FBXLoader**: 펀치 애니메이션 로드
- **홀로그램 셰이더**: Fresnel + 스캔라인 + 글리치 + 전기 오라
- **번개 시스템**: 지그재그 라인 8방향 + 머리 위 흰색 번개

## 🎬 콘텐츠 아이디어
바이브코딩 스쿨 콘텐츠로 만들 때:
- 제목: "피카츄 카드로 진짜 홀로그램 만들기 (코드 받기)"
- 영상: 카드 → 피카츄 등장 → THUNDER PUNCH → 번개
- 설명: "GitHub 링크 공유 → 누구나 자기 폰으로 체험 가능"

⚠️ **라이선스**: 펀치 애니메이션은 Mixamo 등 무료 소스, 피카츄 모델/카드는 닌텐도 IP라 개인 학습용으로만 사용하세요.
