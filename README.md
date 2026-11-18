# LHSG 홈페이지 (www.lhsg.co.kr)

(주)엘에이치에스지 회사 홈페이지입니다. 이 저장소의 `master` 브랜치 루트가 GitHub Pages로 그대로 배포됩니다(Jekyll 사용 안 함, `.nojekyll`).

| 파일 | 내용 |
|---|---|
| `index.html` | 한국어 홈페이지 (`/`) |
| `en/index.html` | 영문 홈페이지 (`/en/`) |
| `privacy.html`, `privacy-en.html` | 모바일 게임 개인정보 처리방침. 앱 등록 정보가 가리키는 주소이므로 옮기거나 지우지 않습니다. |
| `copyright.html` | Shoot & Rush: Multiply 저작권 안내 |
| `app-ads.txt`, `shootnrush/app-ads.txt` | AdMob 인증 파일. 지우지 않습니다. |
| `CNAME` | 연결된 도메인 `www.lhsg.co.kr` |
| `llms.txt` | AI가 읽는 요약 (회사, 일하는 방식, 만든 것, 문의). 홈페이지 문구를 고치면 같이 고칩니다. |
| `about/`, `services/`, `products/`, `portfolio/`, `contact/`, `blog/` | 이전 홈페이지 주소에서 새 홈페이지로 넘기는 페이지 |
| `404.html`, `robots.txt`, `sitemap.xml`, `favicon.*`, `apple-touch-icon.png`, `icon-512.png`, `og-*.png`, `sw.js` | 부속 파일 |

## 문구를 고칠 때

`index.html`과 `en/index.html`에는 같은 본문이 두 번 들어 있습니다(미리 렌더링된 본문과 `<script type="text/x-template">`). 문구를 고칠 때는 두 곳을 모두 고치고, `<head>`의 구조화 데이터(JSON-LD)와 `llms.txt`, `sitemap.xml`의 수정일도 맞춥니다.

## DNS (가비아)

- `www` CNAME → `lhsg.github.io.`
- 루트(`@`) A → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`

이전 홈페이지(Jekyll 블로그 테마)는 이 교체 커밋 이전의 기록에 남아 있습니다.
