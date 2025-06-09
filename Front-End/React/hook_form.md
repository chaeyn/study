```tsx
import { useForm } from "react-hook-form";

type LoginFormInputs = {
  username: string;
  password: string;
};

const {
  register,
  handleSubmit,
  formState: { errors },
} = useForm<LoginFormInputs>();
// React Hook Form에서 폼의 상태와 기능을 관리하는 훅
```

```tsx
<S.Input
  placeholder='아이디를 입력하세요.'
  {...register("username", { required: "아이디를 입력하세요." })}
/>
// username이라는 필드를 hook form에 등록,
// required 옵션을 주면 값이 없을 때 에러 메시지를 자동으로 관리함
```

```tsx
{
  errors.username && (
    <span style={{ color: "red", fontSize: "0.85rem", marginLeft: "5px" }}>
      {errors.username.message}
    </span>
  );
}
// errors.username에 값이 있으면 에러 메시지를 화면에 표시
```
