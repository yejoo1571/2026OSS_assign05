## Deployment

**Vercel 배포 URL** : https://2026ossassign05-seven.vercel.app/

## Key Learning
1. DOM 조작: JavaScript로 HTML 요소를 동적으로 생성하고, 상태 변화에 따라 화면을 다시 그리는 'render()' 패턴의 이해
2. CRUD : 영화 데이터의 생성, 조회, 수정, 삭제 로직 구현 및 데이터 지속성 처리
3. JavaScript 이벤트 및 배열 처리 : addEventListener()를 활용하여 사용자의 입력과 버튼 클릭 등의 이벤트를 처리하고, 배열 메서드를 활용하여 영화 데이터를 관리하는 방법을 학습

## CRUD Service
1. 구현한 서비스 주제 : 사용자가 관람한 영화 제목, 감독, 장르, 평점을 등록하고 수정, 삭제할 수 있습니다.

2. 사용하는 데이터 Field
'id', 'number', 'title', 'director', 'rating', 'genre'

3. Create / Read / Update / Delete 구현 방법
- Create : 입력 폼 제출 시 Form 데이터 객체 생성 후 데이터 배열에 'push()', 'render()' 호출
- Read : 페이지 로드 시 데이터를 읽어와 배열 상태로 복원 후 'render()'를 수행하여 화면에 시각화
- Update : 특정 영화 항목의 '수정' 버튼 클릭 시 폼에 기존 데이터를 로드, 수정 후 해당 'id'를 겁색하여 데이터 갱신 및 'render()'
- Delete : '삭제' 버튼 클릭 시 해당 'id'를 가진 데이터를 배열에서 제거

## JavaScript
- 'document.querySelector()' : DOM 내의 Form, Input 등 특정 HTML 요소를 탐색 및 참조하기 위해 사용
- 'addEventListener()' : Form의 'submit', 버튼의 'click' 등 사용자 상호작용 이벤트를 감지하고 처리
- 'document.createElement()' : 새로운 영화 카드 요소를 동적으로 생성하기 위해 사용
- 'appendChild()' : 생성된 영화 카드 DOM 노드를 상위 컨테이너 요소에 추가
- 'Array Methods'
    - 'forEach' : 영화 데이터 목록을 순회하며 HTML 카드 생성
    - 'filter' : 영화 삭제 기능 구현 시 해당 ID를 제외한 새 배열 생성
- 'render()' : 상태가 변경될 때마다 최신 데이터를 기반으로 UI를 다시 그려 화면을 동기화

## AI / Search Usage

1. 사용한 AI 또는 검색 도구
- Gemini

2. 어떤 문제를 해결하기 위해 사용했는지
- JavaScript에 필요한 기능 질문
- 함수 또는 기능이 적용되지 않는 이유 질문
- 오류 원인 확인 및 해결 방법

3. 실제 코드에 어떻게 적용했는지
- DOM의 필요 기능을 질문하고 사용 방법을 익힌 후 적용
- 삭제 버튼 기능을 만들며 적용되지 않는 이유에 대해 질문하고 해결 방법을 적용

4. 새롭게 이해한 내용
- DOM 요소를 매번 새로 만들지 않고 상위 이벤트 리스너 하나로 하위 요소 이벤트를 제어하는 이벤트 위임 패턴의 효율성을 배움
- DOM에 필요한 다양한 필요 기능에 대해 질문하고 적용하며 배움

## Problem & Solution

### 문제 1 : Update 기능 구현 어려움
- 원인 : 수정 기능 구현에 대해서 단순 조회나 생성 기능과 달리 조금 어려움이 있었습니다.
- 해결 : 수정 기능에 대해서 구현한 후 적용이 안되는 이유, 구현의 문제가 무엇인지 AI에게 질문하며 수정하였습니다.

## Reflection
- 새롭게 알게 된 점 또는 궁금한 점 : DOM의 필요 기능을 찾아보고 적용하며 다양한 기능에 대해서 알게 되었습니다. 