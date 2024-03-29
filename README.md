# goorm-study-description

- **풀스택 6회차 2차 스터디**

## 스터디 개요

### 📅 기간

- 2차 스터디 기간 (언젠지 잘 모름)

### ⛑️ 인원

- **최대인원 : 4명**

- **현재인원**

<a href="https://github.com/kangsinbeom" >
<img src="https://github.com/kangsinbeom.png" width="100" height="100"/>
</a>

### 🚗 스터디 방향성

1. **스스로 하고자 하는 분들이 모여서 머리로만 하는 개발이 아닌 손으로도 하는 공부 구현 위주의 스터디**

2. **아쉽지만 프론트앤드만 모여주세요 (백앤드는 커리큘럼 짤 줄 모름)**

3. **적극적인 코드 리뷰를 통해 지식 공유(코드리뷰 및 발표가 있어 많은 인원은 불가능합니다)**

4. **매일 매일 귀찮게 하지 않기에 본인 스스로가 노력해야 합니다**

<br>
<br>

## 진행 방식 (의논 후 수정 가능 언제든 연락주십셔)

1. 주차별로 1개의 주제에 대해서 구현을 하게 됩니다.

   ex) 1주차: 페이지네이션, 2주차: 인피니티스크롤, 3주차: 검색창 등등...

2. 주제는 단계별로 나누어 필수 사항과 심화 사항으로 나뉘며 필수는 꼭 해야하며 심화는 선택 사항이 됩니다.

   ex) 1단계: 라이브러리를 통한 구현, 2단계: 라이브러리 없이 구현, 3단계: OOO 최적화, 4단계(심화): OOO최적화

3. 중간점검 및 발표일로 주 2회 정기적으로 코드 리뷰를 합니다.

   ex) 수요일: 중간점검일, 토요일: 발표일

4. 중간점검일에는 본인이 구현하면서 있었던 이슈 및 사용한 개념(디자인 패턴, 폴더 구조에 대한 이유, 트러블 슈팅)들에 대해 설명해주며 선택한 이유에 대해서 말하면 되며 문제를 겪고 있는 사항이나 잘 구현되지 않는 부분에 대해서 공유해도 됩니다

5. 발표일에는 최종적으로 구현된 UI와 라이트하우스 및 개발자도구 성능 탭을 살펴보면서 성능향상 및 개선 사항 등 여러 사항에 대해 공유해주시면 됩니다.

## 대표 예시 (이대로 한다는 게 아닙니다!)

### 📂 페이지네이션

### 🛠️ 세팅

**React 세팅: vite**

**스타일 라이브러리: tailwindCSS**

**eslint 및 prettier: 자유**

**전역 상태관리 라이브러리: redux-toolkit**

**비동기 데이터 관리 라이브러리: react-query**

**OpenAPI:**

- [OpenAPI 고양이 사이트](https://thecatapi.com/)
  - 들어가서 내려가지고 Free 버전 사용
  - email로 api key 받기
  - **https://api.thecatapi.com/v1/images/search** 기본 요청
  - 헤더에 받은 X-api-key 꼭 넣기
    - **post man 으로 미리 넘겨서 확인.**
  - 쿼리로 개수제한과 페이지번호를 넘기기
    - 요청부분
      | Name | Type | Description | Default |
      |-------------|------------------|-----------------------------------------------------------------|---------|
      | limit | 1-100 | 반환할 이미지의 개수를 지정합니다. | 1 |
      | page | 0-n | 이미지를 페이지별로 조회할 때 사용할 페이지 번호를 지정합니다. | 0 |
      | order | ASC/DESC/RAND | 이미지를 업로드된 날짜순으로 정렬하는 방식을 지정합니다. | RAND |
      | has_breeds | 1 or 0 | 종 정보가 있는 이미지만 반환합니다. | 0 |
      | breed_ids | 쉼표로 구분된 문자열 | 이미지를 필터링할 특정 종의 ID를 지정합니다. | 없음 |
      | category_ids| 쉼표로 구분된 문자열 | 이미지를 필터링할 특정 카테고리의 ID를 지정합니다. | 없음 |
      | sub_id | 문자열 | 업로드할 때 사용한 sub_id 값을 가진 이미지만 반환합니다. | 없음 |

**통일된 디자인 페이지**

- [웹디자인](https://gsap-flip-grid-view.webflow.io/)
- 리스트 밑에 페이지네이션 기능과 넣으면됌
- 페이지 번호 디자인은 본인 개성따라서
- color는 자유

<br>

**완성조건**

- STEP 1: 데이터를 가져와서 뿌려주기
- STEP 2: 페이징처리를 통한 데이터 불러오기
- STEP 3: 새로고침 시 현재 페이지 고정(처음페이지로 가지 않아야 함)
- STEP 4: 라이브러리 사용시 라이브러이 없이 구현해보기
- STEP 5: 라이트하우스 점수 개선 및 FP /FCP 개선

---

<br>
<br>

## 커리큘럼 (변동 여지 매우 있음 절대 있음!)

- 1주차: firebase 입문
- 2주차: 페이지네이션
- 3주차: 인피니티 스크롤
- 4주차: 검색창
- 5주차: 이미지 최적화

<br>
<br>

여기까지 읽으셨다면 관심이 있어보이십니다. 의견을 많이 피력할 줄 아는 분이면 매우 좋고 조장을 하고 싶다고 하시면 얼마든지 가능하십니다. 뭐든 합의 가능하나 구현과 최적화 위주의 스터디인 것만 알고 계심 됩니다! 많이 알고 계시다고 모시는 게 아니라 소수이기에 의지가 넘치는 사람들을 우선적으로 모셔서 같이 하고 싶습니다! 화이팅~
