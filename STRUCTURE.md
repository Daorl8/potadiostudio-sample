# STRUCTURE · potadiostudio-sample (v0.2)

```
potadiostudio-sample/
├─ index.html              단일 파일 (CSS·JS 인라인)
├─ wrangler.toml           name = potadiostudio-sample → potadiostudio-sample.lgt3232.workers.dev
├─ .assetsignore           img/·문서·v0.1 잔여 파일(pt-hero-*, pt-g-*, pt-round-*)·gamja.png 배포 제외
├─ favicon.png             감자 캐릭터 64px
├─ gamja.webp              감자 캐릭터 (헤더·히어로·테이프·버튼·맨 위로·푸터)
├─ pt-outfit.woff2         영문 (Outfit 500–800)
├─ pt-pretendard.woff2     한글·본문 (Pretendard, 사용 글자만 → 글자 추가 시 재생성)
├─ ix-{studio|record|snap|wedding}.webp   히어로 필름 박스 4프레임
├─ chip-{butter|pink|lav|sky|sage}.webp    02 Record 배경지 칩
├─ st-01~36.webp           01 Studio 갤러리 (img/potadio_studio)
├─ rc-01~32.webp           02 Record 갤러리 (img/potadio_record)
├─ sn-01~32.webp           03 Gamja Snap 갤러리 (img/gamja.snap, 원본 비율)
├─ wd-01~21.webp           04 Wedding 갤러리 (img/forteddy_wedding, 원본 비율)
├─ pt-logo.webp            사장님 노란 로고 (푸터)
├─ og-potadio.jpg          공유 썸네일 1200×630
├─ img/{potadio_studio, potadio_record, gamja.snap, forteddy_wedding}/  다올 제공 원본 (배포 제외)
└─ CHANGELOG.md / STRUCTURE.md
```

## 섹션 순서
헤더 → 히어로(키커 글자만 · `#frames` 4프레임) → 노랑 테이프(`#tape` setInterval 마퀴) → `#studio` 01 → `#record` 02(`#rframe` + `.chip`) → `#snap` 03 → `#wedding` 04 → `#guide` 05 → `#visit` 06 → 푸터 → `#totop`(감자).

## 갤러리
`.grid`(4:5 통일) / `.mas`(메이슨리, 원본 비율) 안 `<figure class="shot">` 한 줄 = 사진 한 장. 처음 장수 = `data-step`, 바로 아래 `.morebtn`으로 같은 수만큼 더 보기. 라이트박스는 같은 챕터 안에서만 넘김.

## 색
`--yellow`(로고 노랑) · `--butter` 가 항상 첫 순서. Record 배경지 `--pink/--lav/--sky/--sage`는 02 챕터와 가격 카드 상단 띠에만.
