# useState

## useState란?

- react 함수형 컴포넌트에서 상태를 관리할 수 있게 해주는 Hook

```tsx
const [count, setCount] = useState(0);

<button onClick={() => setCount(count + 1)}>+1</button>;

// 버튼 클릭 시 setCount를 통해 값이 1씩 증가
```

- 상태 값이 변경되면 컴포넌트가 리렌더링 됨
- 상태 업데이트는 비동기로 처리됨
