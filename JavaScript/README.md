# 변수명 규칙

## `Boolean` 변수명 규칙

`Boolean` 타입의 변수명을 지을 때는 다음의 업데이트된 규칙을 따릅니다

1. **prefix 사용**: 대부분의 경우, 변수명 앞에는 `is`, `has`와 같은 prefix를 붙여 변수의 타입이 `Boolean`임을 명시합니다.

   ```ts
   const isLoading = true;
   const hasChildren = true;
   ```

2. **예외 사항**: `was`, `did`, `can`과 같은 과거형이나 가능성을 직접적으로 표현하는 접두어는 사용하지 않습니다. 이는 주로 현재 상태나 능력보다는 과거 사실이나 일반적인 가능성을 나타내기 때문입니다.
   (`shouldBe`, `will` 등의 미래나 조건을 나타내는 표현도 피합니다.)

3. **특별한 허용**: 일부 상태를 나타내는 단어들은 접두어 없이도 사용할 수 있습니다. 이는 주로 상태를 직접적으로 표현하는 단어들입니다.
   ```ts
   const visible = true;
   const disabled = true;
   const checked = true;
   const active = true;
   ```
