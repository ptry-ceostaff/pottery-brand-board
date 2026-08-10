# POTTERY 브랜드 레퍼런스 보드

포터리 확장 프로젝트용 레퍼런스 브랜드 분류 매트릭스 + 브랜드별 상세 페이지. 직원 교육용.

## 구조

```
index.html      ← 첫 화면 (브랜드 분류 매트릭스, 브랜드 클릭 → 상세)
data/           ← 브랜드별 데이터 (brands.js — 브랜드 1개 = 항목 1개)
brands/         ← (선택) 브랜드별 개별 페이지가 필요할 경우
assets/         ← 로고, 이미지 등
```

## 배포 (깃허브 페이지)

1. 깃허브에서 새 레포 생성 — 이름 예: `pottery-brand-board`, **Private** 권장
2. 이 폴더의 파일 업로드 (웹 UI 드래그 업로드 또는 git push)
3. 레포 **Settings → Pages → Build and deployment**
   - Source: `Deploy from a branch`
   - Branch: `main` / `/ (root)` → Save
4. 1~2분 후 `https://<계정명>.github.io/pottery-brand-board/` 에서 확인

### 접근 제한 주의

- Pro/Team 플랜: 레포가 Private이어도 **배포된 페이지 URL은 공개** (URL을 아는 사람은 접근 가능)
- 조직 멤버만 보기 제한(Pages access control)은 **Enterprise Cloud 플랜** 필요
  - Enterprise인 경우: Settings → Pages → Visibility 를 `Private` 으로

## 콘텐츠 업데이트

브랜드 추가/수정은 `data/brands.js` 항목을 편집 → 커밋하면 페이지에 자동 반영되는 구조로 만든다.
(상세 페이지 템플릿: 한 줄 정의 → 퀵팩트 → 특이사항 → 타임라인 → 상품 구성(잡화·라이프스타일 포함) → 시그니처 & 소비자 반응 → 강점 분석 5축(접기/펼치기) → 포터리 레퍼런스 포인트(라인 태그) → 레퍼런스 이미지)
