# Go Move Prediction AI

딥러닝 텀프로젝트로 만든 **바둑 다음 수 추천 프로그램**입니다.

현재 바둑판 상태를 입력하면 학습된 Residual CNN 모델이 다음 착수 후보 Top-5를 추천합니다.

![Project Cover](assets/cover.png)

## Project

- 주제: 바둑 기보 기반 다음 착수 예측
- 데이터: SGF 바둑 기보
- 모델: Residual CNN Policy Network
- 출력: 19x19 바둑판의 361개 위치 중 추천 착수 Top-5
- 실행: Google Colab에서 저장된 모델을 불러와 웹앱 실행
