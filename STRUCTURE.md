# STRUCTURE · potadiostudio-sample

```
potadiostudio-sample/
├─ index.html              단일 파일 (CSS·JS 인라인)
├─ wrangler.toml           name = potadiostudio-sample → potadiostudio-sample.lgt3232.workers.dev
├─ .assetsignore           img/·문서·index_*.html 배포 제외
├─ pt-outfit.woff2         영문 제목 (Outfit 500–800)
├─ pt-round-r/b/eb.woff2   한글·본문 (나눔스퀘어라운드, 사용 글자만 서브셋 → 글자 추가 시 재생성)
├─ pt-hero-{lavender|pink|sky|mint|butter}.webp   히어로 배경지 칩 사진 5 (1000w)
├─ pt-g-01~75.webp         갤러리 (800w)
├─ pt-logo.webp            사장님 노란 로고 (푸터 타일)
├─ og-potadio.jpg          공유 썸네일 1200×630
├─ img/                    다올 제공 원본 (배포 제외)
└─ CHANGELOG.md / STRUCTURE.md
```

## 섹션 순서
헤더 → 히어로(배경지 칩: `#frame` 사진 + `.chip` 5개, `--bd` 색 변수로 페이지 색 전환) → `#about` → `#price` → `#gallery`(라이트박스 `#lb`) → `#outdoor`(토글 5) → `#guide`(토글 5) → `#visit` → 푸터.

## 색 바꾸기
`:root`의 `--lav/--pink/--sky/--mint/--butter`가 배경지 색. 히어로 칩은 `data-c="var(--…)"`.
