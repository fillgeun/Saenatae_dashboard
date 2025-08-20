# Saenatae_dashboard
On the Internet broadcast, we created a dashboard for team allocation auctions by referring to the auction and bead drawing held at "Chanat'ae (a competition created by capitalism)."

# 🏆 조짜기 경매 대시보드 (Team Draft Auction Dashboard)

> **자낳대 스타일**의 경매 방식으로 팀을 구성하는 실시간 웹 대시보드

20명의 참가자가 경매를 통해 조를 짜는 시뮬레이션 도구입니다. 각 조장이 포인트를 사용해 원하는 선수들을 경매로 영입하고, 남은 선수들은 자율적으로 팀을 선택할 수 있습니다.

## ✨ 주요 기능

- **👥 참가자 관리**: 최대 20명 참가자 등록 및 조장 지정
- **💰 실시간 경매**: 조장들이 1,000 포인트로 선수 경매 진행
- **📊 팀 현황**: 각 팀의 잔여 포인트, 구성원, 인원수 실시간 모니터링
- **🎯 자율 선택**: 경매 종료 후 남은 선수들의 팀 선택
- **📝 진행 로그**: 모든 경매 과정 기록 및 추적
- **💭 실시간 메모**: 경매 진행 중 메모 작성 기능

## 🚀 빠른 시작

1. **파일 다운로드**
   ```bash
   git clone https://github.com/your-username/team-draft-auction
   cd team-draft-auction
   ```

2. **브라우저에서 실행**
   ```
   sujeongbon.html 파일을 브라우저로 드래그하거나 더블클릭
   ```

3. **사용 시작**
   - 참가자 20명 입력
   - 조 개수 및 조장 설정
   - 경매 시작!

## 📖 상세 사용법

### 1단계: 기본 설정
```
참가자 입력 → 조 개수 설정 → 조장 지정 → 설정 적용
```

### 2단계: 경매 진행
```
경매 시작 → 매물 등록 → 입찰 → 낙찰/스킵 → 반복
```

### 3단계: 자율 선택
```
경매 종료 → 자율 선택 시작 → 남은 선수 팀 배정
```

### 주요 규칙
- **초기 포인트**: 각 조장 1,000 포인트
- **입찰 제한**: 잔여 포인트 이내, 현재가보다 높은 금액
- **목표 인원**: 조당 3~8명 (권장: 5명)
- **진행 순서**: 매물 등록 순서대로 경매 진행

## 🛠 기술 스택

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Storage**: Browser Memory (1회성 세션)
- **UI/UX**: Responsive Grid Layout, Dark Theme
- **Browser**: Chrome, Firefox, Safari, Edge 지원

## 📱 화면 구성

```
┌─────────────────────────────────────────────────────────┐
│ Header: 진행 단계 표시                                    │
├─────────────┬─────────────────────┬─────────────────────┤
│ 좌측 (300px)│ 중앙 (가변)          │ 우측 (480px)         │
│             │                    │                    │
│ • 기본 설정  │ • 매물 등록         │ • 팀 현황           │
│ • 참가자 입력│ • 현재 경매         │ • 진행 로그         │
│ • 조 설정   │ • 입찰/낙찰 처리     │ • 실시간 메모       │
│ • 단계 제어 │ • 자율 선택         │                    │
└─────────────┴─────────────────────┴─────────────────────┘
```

## 🎮 사용 시나리오

### 게임/스포츠 팀 구성
- 게임 길드 팀 구성
- 체육대회 조 편성
- 프로젝트 팀 구성

### 교육/행사 운영
- 수업 조 편성
- 워크샵 그룹 구성
- 동아리 팀 나누기

## ⚠️ 주의사항

- **데이터 보존**: 페이지 새로고침 시 모든 데이터 초기화
- **브라우저 호환성**: 모던 브라우저 필요 (IE 11 이하 미지원)
- **동시 접속**: 단일 화면 사용 (멀티플레이어 미지원)

## 🔧 커스터마이징

### 포인트 수정
```javascript
// 초기 포인트 변경 (기본: 1000)
points: 1500  // line ~350
```

### 색상 테마 변경
```css
:root {
  --accent: #6ea8fe;     /* 메인 색상 */
  --accent-2: #22c55e;   /* 성공 색상 */
  --warn: #f59e0b;       /* 경고 색상 */
}
```

### 팀 수 제한 변경
```html
<input type="number" id="teamCount" max="10" />  <!-- 최대 10개 조 -->
```

## 📄 라이선스

```
MIT License - 자유로운 사용, 수정, 배포 가능
```

## 🤝 기여하기

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 문의 및 버그 리포트

- **Issues**: GitHub Issues 탭 활용
- **기능 요청**: Enhancement 라벨로 이슈 등록
- **버그 리포트**: Bug 라벨로 상세 정보와 함께 신고

## 🎯 로드맵

- [ ] **다국어 지원** (English, 日本語)
- [ ] **데이터 내보내기** (JSON, CSV)
- [ ] **팀 밸런스 분석** 기능
- [ ] **모바일 최적화** 
- [ ] **실시간 멀티플레이어** 지원
- [ ] **커스텀 테마** 기능

## 📊 프로젝트 정보

- **버전**: 1.0.0
- **최종 업데이트**: 2025-08-20
- **개발 환경**: HTML5, Vanilla JavaScript
- **라이선스**: MIT
- **AI 생성**: Perplexity AI 어시스턴트 활용

***

**⭐ 도움이 되었다면 Star를 눌러주세요!**

```
Made with ❤️ and AI assistance(perplexity and gemini and chatgpt5)
```