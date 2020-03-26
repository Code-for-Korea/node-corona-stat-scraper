Corona virus stat Scraper for South Korea
===
> 한국 질병관리본부, 연합뉴스에서 통계를 가져옵니다.

DEMO: [JupiterFlow.com](https://jupiterflow.com/corona/api/lastStatus)

## 1. 한국 질병관리본부([링크](http://ncov.mohw.go.kr/bdBoardList_Real.do?brdId=1&brdGubun=13))
> 00시 기준 통계 수치를 10시에 공개합니다.

> type, increment, total, dead, rate, inspection, date

## 2. 연합뉴스([링크](https://www.yna.co.kr/))
> 09시 기준 통계 수치를 14시에 공개합니다.

> totalLast, isolatedLast, deadLast

## 3. 응답 형태
```json
{
    "type":[
      "합계","서울","부산","대구","인천","광주","대전","울산","세종","경기","강원","충북","충남","전북","전남","경북","경남","제주","검역"
    ],
    "increment":[
      "104","13","0","26","1","0","6","0","0","14","0","1","1","0","0","12","0","0","30"
    ],
    "total":[
      "9241","360","112","6482","43","19","30","37","44","401","31","39","124","10","8","1274","90","6","131"
    ],
    "isolated":[
      "4144","80","75","3039","11","11","6","20","8","122","18","14","68","7","3","601","57","4","0"
    ],
    "dead":[
      "131","0","2","94","0","0","0","0","0","4","1","0","0","0","0","30","0","0","0"
    ],
    "rate":[
      "17.82","3.7","3.28","266.04","1.45","1.30","2.04","3.23","12.85","3.03","2.01","2.44","5.84","0.55","0.43","47.85","2.68","0.89","-"
    ],
    "date":"20200326",
    "totalLast":"9241",
    "isolatedLast":"4144",
    "deadLast":"131"
}
```