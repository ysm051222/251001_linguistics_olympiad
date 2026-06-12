# 2025-2학기 특별 세션 1: 미니 언어학 올림피아드
2025년 10월 1일, 서울대학교 언어학회 7기 특별세션 1에서 사용된 미니 언어학 올림피아드 문제지입니다.

푸시다가 오류를 발견하신다면 [이메일](ysm051222@snu.ac.kr)으로 문의하여 주십시오.

- 연습문제: 타닥사학어
- #1: 로비아나어
- #2: 스페인어; 무일락어
- #3: 영어; 데저레트 문자
- #4: 나시오이어; 사보사보어
- #5: 팅링어

제작: 유승민, 김강래, 정원준 // 조판: 유승민

조판에 생성형 AI(chatgpt.com)를 사용한 점을 밝힙니다.

## 파일 구조

- `exam.tex`: 통합 문제지
- `answers.tex`: 답안지
- `preamble.tex`: 공통 글꼴, 여백, 머리말/꼬리말, 문제 제목 양식
- `assets/`: 데저레트 필기체 이미지
- `exam.pdf`, `answers.pdf`: 컴파일된 PDF

## 컴파일

XeLaTeX을 사용합니다.

```bash
latexmk -xelatex exam.tex
latexmk -xelatex answers.tex
```

보조 파일 정리는 다음 명령을 사용합니다.

```bash
latexmk -c
```

## 글꼴

한글 본문, 제목, 머리말을 모두 `NanumMyeongjo` 중심으로 설정했습니다. 꼭 필요한 산세리프 fallback만 `NanumBarunGothic`으로 지정했고, 언어 자료와 IPA 기호는 `Charis SIL`을 사용합니다.

### NanumMyeongjo 다운로드
```
sudo apt update
sudo apt install fonts-nanum
fc-cache -fv
```
