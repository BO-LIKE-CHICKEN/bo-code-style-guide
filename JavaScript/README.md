# 변수명 규칙

## 단수와 복수의 구분

변수명을 정할 때, 셀 수 있는 요소들은 그 수량에 따라 단수형과 복수형으로 구분하여 명명합니다.

1.  **단수형(Singular)**: 단일 항목을 나타낼 때 사용합니다.
    예: `user`, `item`, `category`

2.  **복수형(Plural)**: 여러 항목을 나타낼 때는 주로 `s`, `es`, `ves` 등을 붙여 복수형을 만듭니다. 정확한 접미사는 단어에 따라 다르며, 일반적인 영어 문법 규칙을 따릅니다.
    예: `users`, `items`, `categories`

### 배열을 순회하는 경우의 명명 규칙

배열을 순회하면서 각 요소에 대해 작업을 수행할 때는, 되도록 배열의 이름을 복수형으로, 각 요소의 이름을 해당 복수형에 맞는 단수형으로 명명합니다.

```js
const userNames = users.map((user) => user.name);
```

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
