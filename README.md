# UOJH-Hackathon-Client

> 해커톤 원격 제어 공기청정기 대시보드 (React)

해커톤에서 만든 원격 제어 공기청정기의 웹 대시보드다. 2023년에 만들었다. 중계 서버에 WebSocket으로 접속해 보드가 보내는 온도·습도·대기질을 보여 주고 팬을 제어한다.

## 주요 기능
- 공기청정기 연결 상태 표시 (켜짐·꺼짐)
- 온도, 습도, 대기질(좋음·보통·나쁨) 실시간 표시
- 팬 자동 설정 켜기·끄기, 자동이 꺼져 있을 때 팬 수동 켜기·끄기

## 기술 스택
| 영역 | 기술 |
|---|---|
| 언어 | JavaScript |
| 프레임워크 | React 18, Create React App (react-scripts 5), Tailwind CSS 3, react-switch, axios |

## 구조
```
src/
  App.js     WebSocket 연결, 상태 표시, 팬 제어 화면
  index.js   진입점
```

## 실행
```bash
npm install
npm start
```
서버 주소는 `src/App.js`의 `HOST` 상수에 넣는다.

## 관련 저장소
- [UOJH-Hackathon-Server](https://github.com/son-daehyeon/UOJH-Hackathon-Server) — WebSocket 중계 서버 (Spring Boot)
- [UOJH-Hackathon-Arduino](https://github.com/son-daehyeon/UOJH-Hackathon-Arduino) — 센서·팬 제어 펌웨어 (ESP8266)

---
2023 · 개인 프로젝트 · 보관됨
