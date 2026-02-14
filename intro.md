# 금융경제학: 파이썬을 활용한 금융시장과 통화정책의 이해

**저자: 박기영 (연세대 경제학부)**

**출판사: 시그마프레스**

**출판연도: 2026**

```{image} https://img.shields.io/badge/License-CC%20BY%204.0-blue.svg
:alt: License: CC BY 4.0
:target: https://creativecommons.org/licenses/by/4.0/
```

---

## 저장소 소개

이 저장소(repository)는 **『금융경제학: 파이썬을 활용한 금융시장과 통화정책의 이해』** 에 수록된 그림과 실증 분석을 **독자가 직접 재현(replicate)하고 확장**할 수 있도록 만든 파이썬 코드 모음입니다. 

이 저장소의 목적은 단순히 책 속의 결과를 다시 확인하는데 있지 않습니다. 독자들이 **데이터의 표본기간을 바꾸고**, **변수를 추가·제거하고**, **분석 가정을 수정**하면서 금융경제학적 직관을 스스로 형성하는 데 도움을 주는 것을 목표로 합니다.

## 활용 분야

이 저장소는 다음과 같은 용도로 활용될 수 있습니다:

- 학부 화폐금융론 수업
- 대학원 자산가격결정이론 및 매크로-파이낸스 수업
- 개인 프로젝트
- 실증 분석 연습 및 연구 아이디어 탐색

모두 자유롭게 수정·확장하여 사용하기를 권장합니다.

```{note}
📌 책이나 코드에 있는 오류, 개선사항, 의견 등은 [financialeconomicspython@gmail.com](mailto:financialeconomicspython@gmail.com)으로 보내 주세요. 고맙습니다.
```

---

## 저장소 구조

```
FinancialEconomicsPython/book/
├── README.md              ← 저장소 메인 설명
│ 
├── chapters/              ← 각 장의 분석 코드 (Jupyter Notebook)
│   └── FE01_Bubbles.ipynb, FE02_*.ipynb, ...
│ 
├── readings/              ← 추가 읽을거리
│   └── 뉴스 기사, 보고서, 블로그 글
│ 
├── appendix_online/       ← 온라인 부록
│   └── 교재에 없는 추가 내용
│ 
└── utils/                 ← 공통 함수
    ├── nber_utils.py
    ├── plot_utils.py
    └── preamble_core.py
```

### 폴더 설명

- **chapters/**  
  해당 장에 등장하는 주요 그림과 분석을 재현하는 `.ipynb` 파일을 포함하고 있습니다.

- **readings/**  
  각 장에서 다루는 주제와 관련된 신문 기사, 정책 보고서, 블로그 글, 참고할 만한 추가 읽을거리를 정리해 둔 폴더입니다.

- **appendix_online/**  
  책에서 다루지 않은 내용을 수록하고 있습니다.  

- **utils/**  
  데이터 불러오기, 그래프 그리기, 날짜 처리 등 여러 장에서 반복적으로 사용되는 코드를 모아 둔 폴더입니다.  
  독자는 이 폴더의 코드를 모두 이해하지 않아도 각 장의 노트북을 실행할 수 있습니다.

---

## 빠른 시작

```{admonition} 추천 방법
:class: tip
파이썬을 처음 접하는 독자도 쉽게 사용할 수 있도록 **Google Colab 사용을 권장**합니다.
```

대부분의 노트북은 다음과 같은 순서로 구성되어 있습니다:

1. 필요한 패키지 설치
2. 데이터 불러오기
3. 그림 및 실증 분석 재현

자세한 사용법은 [설치 및 사용법](setup.md) 페이지를 참고하세요.

---

## 주요 링크

- 📚 [GitHub 저장소](https://github.com/FinancialEconomicsPython/book)
- 📖 [교재 코드 보기](chapters/README.md)
- 📝 [추가 읽을거리](readings/README.md)
- 📄 [라이선스 및 인용](license.md)
