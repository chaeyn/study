# Alias Type

```tsx
type Player = {
	name: string,
	age?: number
}

// ? 는 있을수도 있고 없을수도 있다
// -> Undifinded or number

const chaeyn : Player = {
	name: "chaeyn"
}
const cormsdud : Player = {
	name: "cormsdud".
	age: 17
}

if (chaeyn.age && chaeyn.age < 10) {
	console.log("나이가 어립니다")
}

// chaeyn.age가 존재해야 (Not Undifinded)
// if문의 조건을 만족
```

## In Function

```tsx
const PlayerMaker = (name: string): Player => ({ name });

const chaeyn = playerMaker("chaeyn");
chaeyn.age = 17;
```
