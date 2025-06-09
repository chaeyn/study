# useEffect

## useEffect란?

- React의 함수형 컴포넌트에서 사용되는 Hook중 하나
- 컴포넌트가 렌더링될 때 마다 Effect, 부수 효과 등을 수행할 수 있게 해주는 함수

---

- 컴포넌트가 마운트(처음 렌더)될 때, reRender될 때, unMount(제거)될 때 코드를 실행할 수 있다.
- API호출, EventListener 등록/해제 등 부수 효과를 처리할 때 사용

Side Effect

- 함수의 입력과 출력 외의 외부 상태를 변경하는 모든 행위(전역 변수, DOM, 네트워크, 콘솔 등)
- React에서 렌더링 과정과 무관한 작업(fetch, EventListener등록)

의존성 배열

- useEffect의 두 번째 인자에 배열을 넣어서 해당 값이 변경될 때에만 Effect가 실행되도록 제어
