---
title: "글쓰기 테스트2"
type : "status"
date: 2023-07-03T02:49:13+02:00
slug: hugo-encrypttest2
tags:
  - "테스트"
---

## 큰글씨

왜 안나오는 거임 ㅠㅠ

## Hugo Encrypt

> password: **2022**

````markdown
{{%/* hugo-encrypt 2022 */%}}
![Night city](https://unsplash.it/1920/1080/?random=1)
{{%/* /hugo-encrypt */%}}
````

{{% hugo-encrypt 2022 %}}
![Night city](https://unsplash.it/1920/1080/?random=1)
{{% /hugo-encrypt %}}

***

## Multi-block encryption

> Default password: **123456**

```markdown
{{%/* hugo-encrypt */%}}`Here is the test content `{{%/* /hugo-encrypt */%}}
```

{{% hugo-encrypt %}}`Here is the test content `{{%/ hugo-encrypt %}}

End...