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

## Demo Features

- 흑/백 번갈아 착수
- AI 추천 Top-5 표시
- 추천 수 클릭 착수
- 마우스 hover 시 흐릿한 돌 미리보기
- 착수 기록 표시

## How To Run

실행에 필요한 최종 파일은 아래 폴더에 있습니다.

```text
최종 결과물(이 파일들만 업로드하면 바로 사용 가능)/
```

해당 폴더의 `README.md`를 참고하면 Colab에서 바로 실행할 수 있습니다.

## Result

최종 모델은 Residual CNN + board symmetry augmentation을 사용했습니다.

| Model | Test Top-1 | Test Top-5 |
|---|---:|---:|
| Baseline CNN | 19.63% | 49.63% |
| Residual CNN + Augmentation | 25.43% | 56.87% |

## Cover Image 넣는 방법

GitHub 메인 README에 사진을 넣으려면:

1. 프로젝트 루트에 `assets` 폴더를 만듭니다.
2. 넣고 싶은 이미지를 `cover.png`라는 이름으로 저장합니다.
3. 경로가 아래처럼 되면 됩니다.

```text
assets/cover.png
```

README에서는 아래 문법으로 이미지가 표시됩니다.

```markdown
![Project Cover](assets/cover.png)
```

파일명이 다르면 README의 이미지 경로도 같이 바꾸면 됩니다.

