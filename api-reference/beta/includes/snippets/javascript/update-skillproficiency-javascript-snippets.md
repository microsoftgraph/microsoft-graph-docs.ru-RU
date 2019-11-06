---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7476c5e90d25d13f7412d34e65503eef43f11b85
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997510"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const skillProficiency = {
  categories: [
    "categories-value"
  ],
  displayName: "displayName-value",
  proficiency: "proficiency-value",
  webUrl: "webUrl-value"
};

let res = await client.api('/me/profile/skills/{id}')
    .version('beta')
    .update(skillProficiency);

```