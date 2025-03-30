# 🗾 2026 도쿄 & 삿포로 여행 지도

Google Maps API를 활용하여 여행 일정, 루트, 추천 장소, 경비 등을 시각화한 웹 지도입니다.  
모바일에서도 반응형으로 잘 보이도록 설계되었습니다.

## 📂 구성 파일

- `index.html`: 메인 지도 페이지 (여행지별 마커 및 일정 포함)
- `README.md`: 사용 설명서

## 🧩 사용법

1. 이 저장소를 클론하거나 다운로드합니다.
2. `index.html` 파일을 브라우저에서 엽니다.
3. 좌측 사이드바에서 날짜별 여행 계획 확인 가능
4. 하단 버튼으로 소요시간 계산 가능 (실시간 Google Directions API)

## 🔐 Google Maps API Key 설정 방법

`index.html` 내 `<script>` 태그에 아래와 같이 작성되어 있습니다:

```html
<script async defer src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY"></script>
```

> 👇 `YOUR_API_KEY` 부분을 본인의 실제 Google API 키로 교체해야 정상 작동합니다.

## ✏️ 커스터마이징

코드 내 아래 부분만 수정하면 **다른 여행지용 지도**로도 쉽게 바꿀 수 있습니다:

```js
const itinerary = [...];        // 여행 루트 정보
const transportTips = {...};    // 교통수단 안내
const arrivalTimes = {...};     // 도착 예상 시간
const recommendations = {...};  // 추천 활동 / 맛집
const dailyCosts = {...};       // 예상 경비
```

## 📱 모바일 대응

- 반응형 웹 디자인 적용
- GitHub Pages 또는 Netlify에 업로드 시 스마트폰에서도 완벽하게 작동

## 📦 배포 예시 (GitHub Pages)

1. 저장소를 `Public`으로 변경
2. `Settings → Pages → Branch: main / root` 설정
3. 발급된 주소로 접속 (예: `https://사용자명.github.io/저장소명/`)
