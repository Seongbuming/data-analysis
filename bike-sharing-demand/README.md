# Bike Sharing Demand

공유 자전거 사용량 예측 [[Kaggle]](https://www.kaggle.com/competitions/bike-sharing-demand/overview)

## 목표

- 워싱턴 D.C.의 Capital Bikeshare 수요를 시간대 별로 예측
- 자전거 대여 수요를 예측하기 위해 과거 사용 패턴과 날씨 데이터를 분석

## 데이터 필드

- 과거 사용 패턴: 시간(hour), 휴일 여부
- 날씨 데이터: 계절, 날씨, 온도, 체감 온도, 습도, 풍속

| 필드 | 내용 |
|-|-|
| `datetime` | 날짜 + 시간 타임스탬프 |
| `season` | 1: 봄, 2: 여름, 3: 가을, 4: 겨울 |
| `holiday` | 휴일 여부 |
| `weateher` | 1: Clear, Few clouds, Partly cloudy, Partly cloudy<br>2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist<br>3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds<br>4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
| `temp` | 섭씨 온도 |
| `atemp` | 섭씨 체감 온도 |
| `humidity` | 습도 |
| `windspeed` | 풍속 |
| **`casual`** | 비회원 대여량 |
| **`registered`** | 회원 대여량 |
| **`count`** | 총 대여량 |

`casual`, `registered`, `count` 필드를 예측해야 한다.

## EDA & 예측

- [bike-sharing-demand.ipynb](./bike-sharing-demand.ipynb)
