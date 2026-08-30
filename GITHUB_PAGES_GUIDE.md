# 선이음-거리맵 GitHub Pages 배포 방법

## 핵심

휴대폰에서 HTML 파일을 직접 열면 주소가 `content://...` 또는 `file://...`로 시작할 수 있습니다.
이 경우 지도는 뜨더라도 내 위치 권한이 막힐 수 있습니다.

따라서 GitHub Pages에 올려 `https://...` 주소로 접속하는 방식을 권장합니다.

## 가장 쉬운 준비

`suneum-distance-map-github-pages-ready-v0.1.3.zip`을 사용하세요.

압축을 풀면 바로 아래 파일이 보입니다.

- `index.html`
- `sample_polling_places.xlsx`
- `sample_polling_places.csv`
- `README.md`
- `GITHUB_PAGES_GUIDE.md`

이 중 `index.html`은 모바일 단일 실행판입니다.
따라서 GitHub Pages에 올렸을 때 바로 거리맵이 열립니다.

## 휴대폰에서 작업할 때 주의

GitHub 앱에서는 저장소 확인은 편하지만 Pages 설정이 불편할 수 있습니다.

가능하면 다음 방식으로 진행하세요.

1. Chrome 또는 Samsung Internet 실행
2. `https://github.com` 접속
3. 로그인
4. 브라우저 메뉴에서 `데스크톱 사이트` 켜기

## 저장소 만들기

1. GitHub 오른쪽 위 `+` 선택
2. `New repository` 선택
3. Repository name 입력
   - 예: `suneum-distance-map`
4. `Public` 선택
5. `Create repository` 선택

## 파일 올리기

1. 만든 저장소로 이동
2. `Add file` 선택
3. `Upload files` 선택
4. 압축을 푼 파일을 올립니다.
   - `index.html`
   - `sample_polling_places.xlsx`
   - `sample_polling_places.csv`
   - `README.md`
   - `GITHUB_PAGES_GUIDE.md`
5. 아래쪽 `Commit changes` 선택

## GitHub Pages 켜기

1. 저장소 상단 `Settings`
2. 왼쪽 메뉴 `Pages`
3. `Build and deployment` 확인
4. `Source`를 `Deploy from a branch`로 선택
5. `Branch`는 `main`
6. 폴더는 `/root`
7. `Save`

## 접속 주소

몇 분 뒤 아래 형태의 주소가 만들어집니다.

```text
https://본인아이디.github.io/suneum-distance-map/
```

이 주소를 휴대폰 Chrome에서 열면 됩니다.

## 내 위치 권한 확인

1. 거리맵 접속
2. `내 위치` 선택
3. 위치 권한 요청이 뜨면 `허용`

그래도 안 되면 Chrome 설정에서 위치 권한을 확인하세요.

```text
Chrome 설정 > 사이트 설정 > 위치 > github.io 허용
```

현장에서 GPS가 계속 안 잡히면 거리맵의 `위치 찍기`를 사용하세요.
지도에서 문제 장소를 직접 누르면 선택 투표소와의 거리가 계산됩니다.
