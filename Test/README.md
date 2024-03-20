# 테스트 코드 작성 가이드

이 문서에서는 테스트 코드를 작성하는 판단 기준을 다루고 있습니다. 기준과 근거는 다음과 같은 글과 활동에서 학습했던 내용을 기반으로 개인에 맞추어 정리했습니다. 이 과정에서 바뀐 부분이 있을 수 있습니다.

- [2024년 구름톤 3월 COMMIT 프론트엔드 테스팅과 설계](https://tech.goorm.io/2404_commit/)

# 기능과 구현을 나눠서 생각하자

기능과 구현을 나눠서 생각하며, 기능을 테스트 하고 구현이 드러나지 않도록 하자

## 기능이란?

코드를 사용자가 사용할 때 동작을 의미합니다.

> 카운트 버튼을 클릭하면 숫자가 1 올라간다.

## 구현이란?

코드가 어떻게 구현되어 있는지를 의미합니다.

> 카운트를 클릭하면 `state`로 관리되는 `count`라는 값이 이전 값에서 +1 증가한다.