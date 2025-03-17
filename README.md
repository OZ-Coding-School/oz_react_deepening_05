- **주제 : `state`, `props`, `function`을 제작하여 장바구니 완성하기**
- 학습 목표
    1. Props의 구체적인 활용을 다뤄본다.
    2. State의 구체적인 활용을 다뤄본다.
    3. 객체 데이터를 활용하여 화면을 렌더링 한다.
    
- 복습할 개념 체크 리스트
    - [ ]  **React가 데이터를 관리하는 방식**
    설명: React가 데이터를 관리하는 방식에 대해 복습하세요.
    - [ ]  **Props의 개념과 사용하는 방법**
    설명: Props의 개념과 사용하는 방법에 대해 복습하세요.
    - [ ]  **React에서 객체 데이터, 배열 데이터를 다루는 방법**
    설명: 여러 메서드를 활용해 데이터를 다루는 방법에 대해 복습하세요.

- `App.jsx` 컴포넌트 내 요구 사항
    - 전체 화면을 구성하는 컴포넌트 입니다.
    - 카트에 상품을 추가하는 함수 `addToCart` 를 완성하세요.
    - 상품은 **배열객체**로 이루어져 있습니다.
    
- `ProductList.jsx` 컴포넌트 내 요구사항
    - 상품 목록 리스트를 구성하는 컴포넌트 입니다.
    - 이미지 데이터를 각 데이터에 맞게 구성하세요.
        - 이미지 데이터는 `public`폴더에 존재합니다.
        - 각 이미지는 `id`와 동일한 번호입니다. `ex) 01.png`
    - `ProductCard.jsx`를 활용해서 상품을 렌더링 해야 합니다.
        - `Array.map()`을 활용하여 구현 해야 합니다.
        - `ProductCard.jsx` 컴포넌트의 `props`를 참고하여 알맞는 props를 제공 해야 합니다.

- `Cart.jsx` 컴포넌트 내 요구사항
    - 장바구니를 구성하는 컴포넌트 입니다.
    - 장바구니를 열고 닫는 함수 `toggleCart`를 완성하세요.
        - `useState` 를 활용해 `isOpen`의 `State` 를 수정 하세요
    - 장바구니 상품의 가격을 계산하는 `totalPrice`를 완성하세요
        - `Array.reduce()` 를 활용하여 구현합니다.
        - [참고 자료](https://zzang9iu.tistory.com/61)
    - 결제하기 버튼이 동작하는 `handlePurchase` 함수를 완성하세요.
        - 결제하기 버튼을 눌렀을 때 alert를 띄웁니다.
        - 장바구니를 비워야 합니다.
    - **(선택)** 상품 가격에 서식을 지정하는 `totalPriceFormatted` 함수를 완성하세요.
        - 가격 3자리마다 콤마 `,` 를 찍어주는 함수를 작성하세요.
        - 예시) 1000000 → 1,000,000
        - [참고 자료](https://shape-coding.tistory.com/72)
        

- **기본 요구 사항**
    1. `npm install & npm run dev` 를 터미널에 입력하여 서버를 실행합니다. 
    2. `App.jsx` → `ProductList.jsx` → `Cart.jsx` 순서로 구현합니다.
    3. 문제의 **요구 사항**에 대해 구현합니다.
    4. css는 자유롭게 수정해도 좋습니다.
