---
title: "글쓰기 테스트"
type : "status"
date: 2023-07-01T02:49:13+02:00
slug: hugo-encrypttest 
tags:
  - "테스트"
---

## 큰글씨

왜안나와 ㅠㅠ

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