## Node.Js 기반 Open Api를 활용한 소프트웨어 개발자 양성 과정 첫번째 팀 프로젝트 공식 문서

<br/>

**계측 정보 대시보드(전기 사용량)** 전기사용량 데이터를 기반으로 전기요금제 시뮬레이션을 주제로 구현한 대시 보드입니다.<br>

<br/>

## 🚩 목차

- [주제 선택](#-주제-선택)
- [참여 인원](#-참여-인원)
- [코드 작성시 규칙](#-주요-사용-기술)
- [주요 데이터 구조](#-주요-사용-기술)
- [주요 사용 기술](#-주요-사용-기술)
- [디렉토리 구조](#-디렉토리-구조)

<br/>

## 🚩 주제 선택

| 선택 | 팀주제명                | 핵심투입자원       |
| ---- | ----------------------- | ------------------ |
| [ ]  | 네트워크 관리 대시 보드 | D3.js / Ajax / OOP |
| [O]  | 계측 정보 대시 보드     | P5.js / Rest / OOP |

<br/>

## 👷 참여 인원

| 이름   | 파트              | 설명                                                  |
| ------ | ----------------- | ----------------------------------------------------- |
| 안희원 | 반응형 제작 / Api | 반응형 웹 제작 및 json 설계 및 제작                   |
| 서예인 | 프론트엔드 / 기획 | 프론트엔드 로직 / 기획 밎 디자인 레퍼런스 제공        |
| 양정인 | 프론트엔드 / 기획 | 프론트엔드 로직 / 기획 밎 디자인 레퍼런스 제공        |
| 엄정근 | 프론트엔드 / Api  | 프론트엔드 구조 설계 및 로직 처리 / json 설계 및 제작 |

<br/>

## 🔧 개발 환경 셋팅

모든 경로는 root( teamProject )를 기준으로 합니다.

<br/>

## 프론트엔드

1. pug -w ./fontEnd -o ./fontEnd/build -P

> pug 자동 컴파일러

2. sass --watch ./frontEnd/style/scss/index.scss:./frontEnd/style/scss/index.css

> sass 자동 컴파일러

<br />

## 백엔드

1. npm start

> json 서버 실행 ( !package.json에서 port 번호 변경 )

<br />

## 🔧 코드 작성시 규칙

1. 주석은 아래와 같이 작성합니다.

```javascript

/**
 * 사용자 이름 변수
 * @type { String }
 */
let myString = "";


/**
 * 두 매개변수를 더하는 함수
 * ( 2024.02.23 안희원 작성 )
 *
 * @param { Number } sum1 - 첫번째 매개변수
 * @param { Number } sum2 - 두번째 매개변수
 * @return { Number } 두 숫자를 합한 결괏값
 */
const sumFunction = (sum1, sum2) => {
  return sum1 + sum2
}
```

<br/>

## 🔧 주요 데이터 구조

사용되는 데이터(json, rest api, ...) 구조의 관련된 내용을 적어주세요.

```Javascript

// 예시 문서
{
    "month": [
        {
            "id": "month_1",
            "month_data": 1,
            "dong": [
                {
                    "id": "dong_0",
                    "name": 101,
                    "footage": 28,
                    "area": 89.9,
                    "kwh": 84563
                },
                {
                    "id": "dong_1",
                    "name": 102,
                    "footage": 28,
                    "area": 89.9,
                    "kwh": 115414
                },
                {
                    "id": "dong_2",
                    "name": 103,
                    "footage": 32,
                    "area": 105.79,
                    "kwh": 91254
                },
                {
                    "id": "dong_3",
                    "name": 104,
                    "footage": 40,
                    "area": 132.23,
                    "kwh": 75191
                },
                {
                    "id": "dong_4",
                    "name": 105,
                    "footage": 45,
                    "area": 148.76,
                    "kwh": 85842
                }
            ]
        }
    ]
}
```

<br/>

## 🎨 주요 사용 기술

`Front-end`

- JavaScript
- HTML
- SCSS
- PUG
- Bootstrap

`Back-end`

- rest
- json

<br>

## ♻ 디렉토리 구조

```
    .
    └── src
         ├── node_modules
         ├── backEnd (백엔드 관련 디렉토리)
         │     └── database.json
         └── frontEnd (프론트 관련 디렉토리)
                ├── build (pug build)
                │    └── index.html
                ├─── js (JS 관련 디렉토리)
                │    ├── admin.js (admin)
                │    ├── chart.js (chart)
                │    └── index.js (summary)
                ├─── style (style 관련 디렉토리)
                │      ├── image
                │      └── scss (scss 관련 디렉토리)
                │            ├── index.css
                │            ├── index.css.map
                │            └── index.scss
                └─── index.pug

```

<br/>
