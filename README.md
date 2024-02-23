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
| 임정근 | 프론트엔드 / Api  | 프론트엔드 구조 설계 및 로직 처리 / json 설계 및 제작 |

<br/>

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

```Json

// 예시 문서
{
    "popularNo3" : [
        {
            "week" : 1, // 주 차
            "weekData" : [ // 주 차에 관련된 데이터
                { "Rank" : 1, "Singer" : "zard", "Title" : "LUV" }, // Rank == 랭킹, Singer == 가수, Title == 제목
                { "Rank" : 2, "Singer" : "BlackPink", "Title" : "HOW YOU LIKE THAT" },
                { "Rank" : 3, "Singer" : "IVE", "Title" : "I AM" }
            ]
        },
        {
            "week" : 2,
            "weekData" : [
                { "Rank" : 1, "Singer" : "IVE", "Title" : "I AM" },
                { "Rank" : 2, "Singer" : "ZARD", "Title" : "LUV" },
                { "Rank" : 3, "Singer" : "AESPA", "Title" : "SPICY" }
            ]
        },
        {
            "week" : 3,
            "weekData" : [
                { "Rank" : 1, "Singer" : "zard", "Title" : "LUV" },
                { "Rank" : 2, "Singer" : "IVE", "Title" : "I AM" },
                { "Rank" : 3, "Singer" : "NewJeans", "Title" : "Hype Boy" }
            ]
        },
        {
            "week" : 4,
            "weekData" : [
                { "Rank" : 1, "Singer" : "AESPA", "Title" : "SPICY" },
                { "Rank" : 2, "Singer" : "IVE", "Title" : "I AM" },
                { "Rank" : 3, "Singer" : "NewJeans", "Title" : "Hype Boy" }
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
         ├── build (pug 빌드 디렉토리)
         │     └── index.html
         ├── style (스타일 관련 디렉토리)
         │     ├── scss (스타일 시트 관련 디렉토리)
         │     └── image (이미지 관련 디렉토리)
         ├── js (자바스크립트 관련 디렉토리)
         └── index.pug
```

<br/>
