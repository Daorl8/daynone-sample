# STRUCTURE — daynone-sample

## 배포
- 레포: github.com/Daorl8/daynone-sample → Cloudflare 연결 → daynone-sample.lgt3232.workers.dev
- 단일 파일 정적 사이트. `wrangler.toml`(name=daynone-sample, [assets] directory="./") + `.assetsignore`.

## 파일
- `index.html` — 전체 사이트(CSS·JS 인라인). 단일 파일.
- `dn-*.jpg` — self-host 이미지 18종:
  - dn-hero(히어로 내부), dn-sign-night/dn-sign-day(간판), dn-logo/dn-card(브랜드)
  - dn-coffee/dn-ice/dn-cups/dn-tea(낮), dn-wine/dn-cocktail/dn-blue/dn-plate(밤)
  - dn-ppl/dn-outdoor/dn-dessert(공간·무드), dn-reserved(예약), dn-dog(반려견, 현재 미사용)
- `CHANGELOG.md` / `STRUCTURE.md` — 문서(서빙 제외, .assetsignore).

## 폰트
- Fraunces(디스플레이, CDN) + Pretendard(본문, CDN). 납품 확정 시 self-host 전환 예정.

## 원본 소스
- IG 원본 이미지(hash 파일명)는 로컬 daynone-sample 폴더에 보관, 레포엔 dn-*.jpg만 커밋.
