# Sonawave

Sonawave 홈페이지 소스입니다. GitHub Pages로 배포되는 정적 사이트입니다.

- 공개 주소: https://hisona.github.io/Sonawave/
- 진입 파일: [index.html](index.html) — HTML 한 파일에 CSS가 포함되어 있고 외부 요청이 없습니다.
- 로고: [images/sonawave_logo.png](images/sonawave_logo.png)

## 구성

| 섹션 | 내용 |
| --- | --- |
| Hero | 로고와 슬로건 |
| 앱 | ADSFile, ADS Player, Golf Form Caddie 요약 |
| 사업 영역 | Google Play 앱 개발·배포, Apple App Store 앱 개발·배포, 통신판매업·전자상거래, 소프트웨어 개발 및 기술 서비스 |
| 사업자 정보 | 전자상거래법 표시 항목 |
| 문의 | 메일, GitHub |

## 배포

GitHub Pages 설정에서 소스를 `main` 브랜치의 `/ (root)` 로 지정하면 됩니다.
`.nojekyll` 파일이 있어 Jekyll 처리 없이 파일이 그대로 서빙됩니다.

```bash
git add -A && git commit -m "Add Sonawave homepage" && git push
```

로컬 확인:

```bash
python3 -m http.server 8000
```

## 배포 전 채워야 할 항목

`index.html` 의 `#company` 표에 실제 값을 넣어야 합니다. 현재는 자리표시자입니다.

- 대표자
- 사업자등록번호
- 통신판매업 신고번호
- 사업장 주소

통신판매업 신고번호는 [공정거래위원회 통신판매사업자 조회](https://www.ftc.go.kr/bizCommPop.do)
링크와 함께 표시하는 것이 일반적입니다.
