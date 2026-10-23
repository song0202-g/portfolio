# 빅데이터 분석 포트폴리오

GitHub Pages로 바로 배포되는 정적 웹사이트입니다. 빌드 과정이나 Node.js 설치 없이 파일만 올리면 됩니다.

## 폴더 구조

```
index.html        ← 페이지 전체 (본문, 디자인, 애니메이션이 모두 이 파일 하나에 들어 있음)
images/           ← 프로젝트 결과 이미지
.nojekyll         ← GitHub Pages 설정용 (지우지 마세요)
```

## 배포 방법 (GitHub Pages)

1. 이미 있는 `song0202-g/portfolio` 저장소를 쓰면 주소는 `https://song0202-g.github.io/portfolio/` 입니다. 기존 `index.html`, `portfolio-preview.html`, `profile-photo.png`는 이번 파일로 교체하거나 지워도 됩니다. (새로 만든다면: 저장소를 만듭니다. 이름을 `아이디.github.io`로 하면 주소가 `https://아이디.github.io`가 됩니다. 다른 이름이면 `https://아이디.github.io/저장소이름`이 됩니다.)
2. 저장소 페이지에서 **Add file → Upload files**를 눌러 이 폴더 안의 파일을 모두 끌어다 놓고 **Commit changes**.
   (`.nojekyll`처럼 점으로 시작하는 파일이 안 보이면 Mac은 `Cmd+Shift+.`, Windows는 탐색기 "숨긴 항목" 체크)
3. **Settings → Pages**에서 Source를 **Deploy from a branch**, Branch를 **main / (root)** 로 선택 후 Save.
4. 1~2분 뒤 위 주소로 접속하면 포트폴리오가 보입니다.

## 꼭 바꿔야 할 곳

| 항목 | 위치 |
|---|---|
| 프로젝트별 GitHub 링크 | `index.html` — Project 01 `low-light-enhancement`, Project 02 `inbound-tourism-forecast` 저장소로 연결됨 |
| 이메일 | `index.html` 첫 화면 인적사항 패널의 Email 줄 |

## 프로젝트 이미지 · 영상

**Project 01 (저조도 영상 개선)** 은 영상 3개가 이미 들어가 있습니다. 화면에 보이면 소리 없이 자동 재생되고, 세 영상의 시간이 맞춰져 같은 장면을 비교할 수 있습니다.

| 파일 | 내용 |
|---|---|
| `p1-trifusesimple.mp4 / .webm / .jpg` | 직접 구현 모델(TriFuseSimple) 결과 — 큰 화면 |
| `p1-original.mp4 / .webm / .jpg` | 원본 저조도 입력 영상 |
| `p1-trifuselite.mp4 / .webm / .jpg` | 기존 모델(TriFuseLite) 결과 |

(mp4는 Chrome·Safari·Edge용, webm은 그 외 브라우저용 예비 파일, jpg는 로딩 전 미리보기 이미지입니다.)

**Project 02 (방한 관광 입국자 수 예측)** 는 분석 노트북에서 저장한 그래프 3장이 들어가 있습니다.

| 파일 | 내용 |
|---|---|
| `p2-1.png` | 관광(tour) 원계열 ACF · PACF |
| `p2-2.png` | 차분(d=1, D=1) 후 ACF · PACF |
| `p2-3.png` | 관광 SARIMA(1,1,2)(0,1,1,12) 예측 그래프 (로그 전체 구간 + 2023~2024 실제 인원) |

같은 이름으로 더 선명한 이미지를 덮어쓰면 그대로 바뀝니다.

## 로컬에서 미리보기

zip 압축을 **먼저 풀고** 폴더 안의 `index.html`을 더블클릭하면 됩니다.
(영상과 이미지는 압축을 푼 폴더의 `images/`에 있어야 보입니다.)
