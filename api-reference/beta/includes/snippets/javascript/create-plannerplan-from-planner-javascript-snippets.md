---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8c28808292b10be2b2506fdb0ac2fca3ce17989f
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2019
ms.locfileid: "36638391"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  owner: "ebf3b108-5234-4e22-b93d-656d7dae5874",
  title: "title-value"
};

let res = await client.api('/planner/plans')
    .version('beta')
    .post(plannerPlan);

```