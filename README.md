# 🐍 파이썬 튜토리얼 — 처음부터 배우는 Python

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

파이썬을 처음 시작하는 분들을 위한 **단계별 실습 튜토리얼**입니다.
각 강의는 Jupyter 노트북(`.ipynb`) 형태로 되어 있어, 코드를 직접 실행하면서 학습할 수 있습니다.

---

## 📋 사전 준비

### 1. Python 설치 확인

이미 Python 3.10 이상이 설치되어 있다면 [Jupyter 설치](#2-jupyter-설치)로 이동하세요.

#### Windows에서 Python 설치 여부 확인

1. **시작 메뉴** → **명령 프롬프트** 또는 **PowerShell** 열기
2. 다음 명령 입력:

```
python --version
```

3. `Python 3.10.x` 이상이 표시되면 설치 완료

> ⚠️ `python` 명령이 인식되지 않으면 Python이 설치되지 않은 것입니다.

#### Python이 없는 경우 — Anaconda 설치 (권장)

**Anaconda**는 Python + 주요 라이브러리 + Jupyter를 한 번에 설치해 주는 배포판입니다.

1. **Anaconda 다운로드 페이지**에 접속:
   - https://www.anaconda.com/download
2. **Windows** 버전 다운로드 (64-bit)
3. 다운로드한 설치 파일(`Anaconda3-xxxx-Windows-x86_64.exe`) 실행
4. 설치 옵션:
   - ✅ **Just Me (recommended)** 선택
   - ✅ **Add Anaconda to my PATH environment variable** 체크 (중요!)
   - ✅ **Register Anaconda as default Python** 체크
5. **Install** 클릭 → 설치 완료 대기 (약 5~10분)
6. 설치 완료 후 명령 프롬프트에서 확인:

```
python --version
conda --version
```

> 💡 **Anaconda 대신 Miniconda**: 디스크 공간이 부족하면 [Miniconda](https://docs.conda.io/en/latest/miniconda.html)(최소 설치판)를 사용하세요.

---
### 2. Jupyter 설치

#### Anaconda를 설치한 경우

Jupyter가 이미 포함되어 있습니다. 바로 [Jupyter 실행](#3-jupyter-실행하기)으로 이동하세요.

#### Python만 설치한 경우 (pip 사용)

명령 프롬프트를 열고 다음 명령 실행:

```bash
pip install jupyter
```

설치 확인:

```bash
jupyter --version
```

---

### 3. Jupyter 실행하기

#### 방법 A: 명령 프롬프트에서 실행 (권장)

1. 명령 프롬프트(또는 Anaconda Prompt) 열기
2. 튜토리얼 폴더로 이동:

```bash
cd your-directory
```

3. Jupyter Lab 실행 (권장):

```bash
jupyter lab
```

또는 Jupyter Notebook 실행:

```bash
jupyter notebook
```

4. 브라우저가 자동으로 열립니다 (보통 `http://localhost:8888/lab`)

#### 방법 B: VS Code에서 실행

1. VS Code 설치: https://code.visualstudio.com/
2. **Python 확장** 설치 (확장 탭에서 "Python" 검색)
3. **Jupyter 확장** 설치 (확장 탭에서 "Jupyter" 검색)
4. 폴더 열기: **파일** → **폴더 열기** → `your-directory`
5. `.ipynb` 파일 클릭 → 노트북이 자동으로 열립니다

#### 방법 C: Anaconda Navigator에서 실행

1. **시작 메뉴** → **Anaconda Navigator** 실행
2. **Jupyter Lab** 또는 **Jupyter Notebook**의 **Launch** 버튼 클릭
3. 브라우저에서 해당 폴더로 이동

---

## 📖 노트북 사용법

### 셀(Cell)이란?

Jupyter 노트북은 **셀(Cell)**이라는 작은 블록들로 구성됩니다.

| 셀 종류 | 용도 | 실행 방법 |
|---------|------|-----------|
| **마크다운 셀** | 설명 글, 제목, 표 | 실행해도 결과 없음 |
| **코드 셀** | 파이썬 코드 | `Shift + Enter`로 실행 |

### 기본 조작

| 단축키 | 동작 |
|--------|------|
| `Shift + Enter` | 현재 셀 실행하고 다음 셀로 이동 |
| `Ctrl + Enter` | 현재 셀만 실행 |
| `A` (명령 모드) | 위에 새 셀 삽입 |
| `B` (명령 모드) | 아래에 새 셀 삽입 |
| `DD` (명령 모드) | 현재 셀 삭제 |
| `M` (명령 모드) | 셀을 마크다운으로 변경 |
| `Y` (명령 모드) | 셀을 코드로 변경 |

> 💡 **명령 모드**는 셀을 선택한 상태(파란색 테두리)에서 동작합니다. 편집 모드(녹색 테두리)에서 `Esc`를 누르면 명령 모드로 전환됩니다.

### 학습 팁

1. **코드 셀을 하나씩 실행**하면서 결과를 확인하세요
2. **값을 수정**해서 다시 실행해 보세요 (예: 숫자 바꾸기, 문자열 바꾸기)
3. **🎯 연습 문제**는 노트북 마지막에 있습니다. 직접 풀어보세요
4. 모르는 것이 있으면 셀 아래에 새 셀을 추가(`B`)해서 실험해 보세요

---

## 🗂️ 커리큘럼

### [01] 변수 — 파이썬 기초

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_변수와_자료형.ipynb` | 변수와 자료형 | 변수 선언, 이름 규칙, type(), None, 자료형 한눈에 보기 |
| 2 | `2_정수와_연산.ipynb` | 정수와 연산자 | 산술/비교/논리/항등/비트 연산자, 진수 표기, 할당 연산자 |
| 3 | `3_불리언과_실수.ipynb` | 불리언과 실수 | True/False, bool() 변환, 부동소수점 오차, inf/NaN |
| 4 | `4_문자열.ipynb` | 문자열 | 인덱싱/슬라이싱, 메서드, 이스케이프, f-string 포매팅 |
| 5 | `5_리스트.ipynb` | 리스트 | 생성/수정/슬라이싱, 정렬, 컴프리헨션, 얕은/깊은 복사 |
| 6 | `6_튜플과_집합.ipynb` | 튜플과 집합 | 튜플 언패킹, set 연산(합/교/차집합), frozenset |
| 7 | `7_딕셔너리와_바이트.ipynb` | 딕셔너리와 바이트 | dict 생성/조작, 반복, 컴프리헨션, bytes/bytearray, 인코딩 |

### [02] 제어 — 흐름 제어

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_if_조건문.ipynb` | if 조건문 | if/elif/else, 중첩 조건, 논리 연산자, in/not in, Truthy/Falsy |
| 2 | `2_for_반복문.ipynb` | for 반복문 | range(), enumerate(), zip(), 딕셔너리 순회, 중첩 for문, for-else |
| 3 | `3_while_반복문.ipynb` | while 반복문 | while 기본, while-else, break/continue, for vs while 비교 |
| 4 | `4_match_case와_삼항연산자.ipynb` | match-case와 삼항 연산자 | 패턴 매칭, OR/타입/리스트/딕셔너리 패턴, 삼항 연산자, 단락 평가, := |
| 5 | `5_예외처리.ipynb` | 예외 처리 | try-except-else-finally, raise, 사용자 정의 예외, 예외 체인 |
| 6 | `6_with문과_컴프리헨션.ipynb` | with문과 컴프리헨션 | with문 파일 관리, 컨텍스트 매니저, 리스트/딕셔너리/집합/제너레이터 컴프리헨션 |

### [03] 함수 — 함수와 고급 기법

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_함수정의와_반환.ipynb` | 함수 정의와 반환값 | def, 매개변수, return, 다중 반환, docstring, 타입 힌트 |
| 2 | `2_매개변수와_인수.ipynb` | 매개변수와 인수 | 위치/키워드 인수, 기본값, mutable 주의점, *args/**kwargs, 위치/키워드 전용 |
| 3 | `3_람다와_고차함수.ipynb` | 람다와 고차 함수 | lambda, map/filter/reduce, sorted+key, 함수를 인수/반환값으로 |
| 4 | `4_스코프와_클로저.ipynb` | 스코프와 클로저 | LEGB 규칙, global/nonlocal, 클로저, 팩토리 패턴 |
| 5 | `5_데코레이터.ipynb` | 데코레이터 | @문법, functools.wraps, 다중 데코레이터, 매개변수 있는 데코레이터 |
| 6 | `6_제너레이터와_재귀.ipynb` | 제너레이터와 재귀 | yield, 제너레이터 표현식, 무한 시퀀스, 파이프라인, 재귀(팩토리얼/피보나치) |
| 7 | `7_내장함수와_고차함수.ipynb` | 내장 함수와 고차 함수 | 타입/수학 내장함수, enumerate/zip/all/any, sorted+key, functools.partial |

### [04] 입출력 — 파일과 환경

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_입력과_출력.ipynb` | 입력과 출력 | input(), 타입 변환, 여러 값 파싱, 입력 검증, print() 옵션 |
| 2 | `2_f_string_포매팅.ipynb` | f-string 포매팅 | f-string 기본, 숫자 포매팅, 정렬, 날짜 포맷, 디버깅 포맷, 구식 포맷팅 비교 |
| 3 | `3_파일입출력.ipynb` | 파일 입출력 | 텍스트 파일 읽기/쓰기, 파일 모드(r/w/a/x), 줄 단위 읽기, writelines() |
| 4 | `4_CSV와_JSON.ipynb` | CSV와 JSON | csv.reader/writer, DictReader/DictWriter, json.dump/load, json.dumps/loads |
| 5 | `5_명령행_인수.ipynb` | 명령행 인수 | sys.argv, argparse 기본/옵션 인수, choices, nargs |
| 6 | `6_환경변수와_설정.ipynb` | 환경변수와 설정 | os.environ, 타입 변환 헬퍼, configparser로 INI 파일 관리 |
| 7 | `7_경로와_디렉토리.ipynb` | 경로와 디렉토리 | os.path, pathlib.Path, 디렉토리 생성/순회, 파일 읽기/쓰기 |
| 8 | `8_로깅.ipynb` | 로깅 | 로깅 레벨, 파일/콘솔 핸들러, 로거 계층, 예외 로깅 |

### [05] 클래스 — 객체 지향 프로그래밍

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_클래스정의와_초기화.ipynb` | 클래스 정의와 초기화 | class, __init__, self, 인스턴스/클래스 속성, __repr__/__str__ |
| 2 | `2_상속.ipynb` | 상속 | 기본 상속, super(), 메서드 오버라이딩, 다중 상속과 MRO, isinstance() |
| 3 | `3_캡슐화.ipynb` | 캡슐화 | public/protected/private, @property, getter/setter, __slots__ |
| 4 | `4_다형성.ipynb` | 다형성 | 상속 기반 다형성, 덕 타이핑, 연산자 오버로딩, ABC 추상 클래스 |
| 5 | `5_메서드와_프로퍼티.ipynb` | 메서드와 프로퍼티 | 인스턴스/클래스/정적 메서드, @classmethod 대체 생성자, @property |
| 6 | `6_매직_메서드.ipynb` | 매직 메서드 | __str__/__repr__/__format__, 비교 연산자, 컨테이너 프로토콜 |
| 7 | `7_데이터클래스.ipynb` | 데이터클래스 | @dataclass, field(), frozen, 상속, asdict/astuple |
| 8 | `8_열거형과_네임드튜플.ipynb` | 열거형과 네임드튜플 | Enum, IntEnum, auto(), NamedTuple, 비교 |

### [06] 모듈 — 표준 라이브러리

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_모듈기초.ipynb` | 모듈 기초 | import 형태, 모듈 속성, 커스텀 모듈, __all__, 조건부 import |
| 2 | `2_패키지와_임포트.ipynb` | 패키지와 임포트 | 패키지 구조, __init__.py, 절대/상대 임포트, sys.path |
| 3 | `3_os와_sys.ipynb` | os와 sys | 환경변수, 경로, 파일/디렉토리, sys.argv, pathlib |
| 4 | `4_collections.ipynb` | collections | Counter, defaultdict, deque, namedtuple |
| 5 | `5_itertools.ipynb` | itertools | count/cycle/repeat, accumulate, chain, permutations/combinations |
| 6 | `6_functools와_datetime.ipynb` | functools와 datetime | reduce, partial, lru_cache, date/time, timedelta |
| 7 | `7_정규표현식.ipynb` | 정규표현식 | 패턴 매칭, 문자 클래스, 수량자, 그룹과 캡처, compile |
| 8 | `8_유틸리티.ipynb` | 유틸리티 | random, math, json 직렬화, hashlib |

### [07] 표준라이브러리 — 표준 라이브러리 심화

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_파일과_경로.ipynb` | 파일과 경로 | pathlib, glob, shutil, zipfile |
| 2 | `2_os와_시스템.ipynb` | os와 시스템 | 환경변수, 파일 시스템, sys.argv, argparse |
| 3 | `3_json과_pickle.ipynb` | JSON과 Pickle | JSON 직렬화/역직렬화, Pickle 객체 저장, 커스텀 직렬화 |
| 4 | `4_시간과_날짜.ipynb` | 시간과 날짜 | time 타임스탬프, datetime, timedelta, 시간 측정 |
| 5 | `5_예외와_트레이스백.ipynb` | 예외와 트레이스백 | try/except, 사용자 정의 예외, traceback 모듈 |
| 6 | `6_타입힌트.ipynb` | 타입 힌트 | 기본/컬렉션 타입, Optional, Callable, TypeVar, Generic |
| 7 | `7_연산자와_해시.ipynb` | 연산자와 해시 | operator 모듈, itemgetter, hashlib, HMAC |
| 8 | `8_URL과_웹.ipynb` | URL과 웹 | urllib 파싱/인코딩, webbrowser, URL 빌더 |

### [11] 기술통계 — 데이터 분석 기초

| # | 노트북 | 주제 | 내용 요약 |
|---|--------|------|----------|
| 1 | `1_변량데이터와_기초통계량.ipynb` | 변량 데이터와 기초 통계량 | NumPy 배열, 합계/평균, 표본분산/불편분산, 표준편차, 표준화, 사분위수 |
| 2 | `2_다변량데이터와_pandas.ipynb` | 다변량 데이터와 pandas | DataFrame, groupby, pivot_table, 교차집계표 |
| 3 | `3_공분산과_상관계수.ipynb` | 공분산과 상관계수 | 공분산, 분산-공분산 행렬, 피어슨 상관계수, 상관행렬 |
| 4 | `4_데이터_시각화.ipynb` | 데이터 시각화 | matplotlib, seaborn, 히스토그램, KDE, boxplot, violin, 산점도, 페어플롯 |

---

## 🔧 자주 묻는 질문 (FAQ)

### Q: Jupyter 실행 시 `jupyter: 명령을 찾을 수 없습니다`라고 나와요

**A:** PATH 설정 문제입니다.

1. Anaconda를 설치했다면 **Anaconda Prompt**에서 실행하세요
2. Python만 설치한 경우:
   ```bash
   python -m notebook
   ```
   또는 PATH에 Python Scripts 폴더를 추가하세요

### Q: 노트북 파일이 열리지 않아요

**A:** Jupyter Lab/Notebook이 실행 중인지 확인하고, 브라우저에서 `http://localhost:8888`에 접속하세요.

### Q: 코드 셀이 실행되지 않아요 (`In [*]` 상태)

**A:** 다른 셀이 실행 중일 수 있습니다.
- 메뉴 → **Kernel** → **Interrupt** 클릭
- 또는 **Kernel** → **Restart & Clear Output** 클릭

### Q: 커널이 연결되지 않아요

**A:** Python 커널이 응답하지 않는 경우:
1. **Kernel** → **Restart** 클릭
2. 그래도 안 되면 **Kernel** → **Restart & Clear Output** 클릭
3. Jupyter를 종료하고 다시 실행

### Q: 한글이 깨져 보여요

**A:** 노트북 파일은 UTF-8로 저장되어 있습니다. Jupyter Lab은 기본적으로 UTF-8을 지원합니다. VS Code에서는 우측 하단의 인코딩이 `UTF-8`인지 확인하세요.

---

## 📂 디렉토리 구조

```
.
├── README.md
├── [01]변수/
│   ├── 1_변수와_자료형.ipynb
│   ├── 2_정수와_연산.ipynb
│   ├── 3_불리언과_실수.ipynb
│   ├── 4_문자열.ipynb
│   ├── 5_리스트.ipynb
│   ├── 6_튜플과_집합.ipynb
│   └── 7_딕셔너리와_바이트.ipynb
├── [02]제어/
│   ├── 1_if_조건문.ipynb
│   ├── 2_for_반복문.ipynb
│   ├── 3_while_반복문.ipynb
│   ├── 4_match_case와_삼항연산자.ipynb
│   ├── 5_예외처리.ipynb
│   └── 6_with문과_컴프리헨션.ipynb
├── [03]함수/
│   ├── 1_함수정의와_반환.ipynb
│   ├── 2_매개변수와_인수.ipynb
│   ├── 3_람다와_고차함수.ipynb
│   ├── 4_스코프와_클로저.ipynb
│   ├── 5_데코레이터.ipynb
│   ├── 6_제너레이터와_재귀.ipynb
│   └── 7_내장함수와_고차함수.ipynb
├── [04]입출력/
│   ├── 1_입력과_출력.ipynb
│   ├── 2_f_string_포매팅.ipynb
│   ├── 3_파일입출력.ipynb
│   ├── 4_CSV와_JSON.ipynb
│   ├── 5_명령행_인수.ipynb
│   ├── 6_환경변수와_설정.ipynb
│   ├── 7_경로와_디렉토리.ipynb
│   └── 8_로깅.ipynb
├── [05]클래스/
│   ├── 1_클래스정의와_초기화.ipynb
│   ├── 2_상속.ipynb
│   ├── 3_캡슐화.ipynb
│   ├── 4_다형성.ipynb
│   ├── 5_메서드와_프로퍼티.ipynb
│   ├── 6_매직_메서드.ipynb
│   ├── 7_데이터클래스.ipynb
│   └── 8_열거형과_네임드튜플.ipynb
├── [06]모듈/
│   ├── 1_모듈기초.ipynb
│   ├── 2_패키지와_임포트.ipynb
│   ├── 3_os와_sys.ipynb
│   ├── 4_collections.ipynb
│   ├── 5_itertools.ipynb
│   ├── 6_functools와_datetime.ipynb
│   ├── 7_정규표현식.ipynb
│   └── 8_유틸리티.ipynb
├── [07]표준라이브러리/
│   ├── 1_파일과_경로.ipynb
│   ├── 2_os와_시스템.ipynb
│   ├── 3_json과_pickle.ipynb
│   ├── 4_시간과_날짜.ipynb
│   ├── 5_예외와_트레이스백.ipynb
│   ├── 6_타입힌트.ipynb
│   ├── 7_연산자와_해시.ipynb
│   └── 8_URL과_웹.ipynb
└── [11]기술통계/
    ├── fish_multi.csv
    ├── shoes.csv
    ├── cov.csv
    ├── fish_multi_2.csv
    ├── 1_변량데이터와_기초통계량.ipynb
    ├── 2_다변량데이터와_pandas.ipynb
    ├── 3_공분산과_상관계수.ipynb
    └── 4_데이터_시각화.ipynb
```

---

## 🎯 학습 추천 순서

1. **[01]변수**를 순서대로 완료 (변수 → 정수 → 불리언/실수 → 문자열 → 리스트 → 튜플/집합 → 딕셔너리)
2. **[02]제어**를 순서대로 완료 (if → for → while → match-case → 예외처리 → with/컴프리헨션)
3. **[03]함수**를 순서대로 완료 (정의 → 매개변수 → 람다 → 스코프 → 데코레이터 → 제너레이터 → 내장함수)
4. **[04]입출력**을 순서대로 완료 (입출력 → f-string → 파일 → CSV/JSON → 명령행 → 환경변수 → 경로 → 로깅)
5. **[05]클래스**를 순서대로 완료 (정의 → 상속 → 캡슐화 → 다형성 → 메서드 → 매직메서드 → 데이터클래스 → Enum/NamedTuple)
6. **[06]모듈**을 순서대로 완료 (모듈기초 → 패키지 → os/sys → collections → itertools → functools/datetime → 정규표현식 → 유틸리티)
7. **[07]표준라이브러리**를 순서대로 완료 (파일과경로 → os/시스템 → JSON/Pickle → 시간/날짜 → 예외/트레이스백 → 타입힌트 → 연산자/해시 → URL/웹)
8. **[11]기술통계**를 순서대로 완료 (변량데이터/기초통계량 → 다변량데이터/pandas → 공분산/상관계수 → 데이터시각화)

> 💡 각 노트북은 앞의 내용을 이해했다는 가정 하에 작성되어 있습니다. 순서대로 학습하세요.

---

## 📝 라이선스

이 튜토리얼은 [MIT License](https://opensource.org/licenses/MIT)로 배포됩니다.
자유롭게 학습하고 공유하세요!