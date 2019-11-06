---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81a293d9d2280a57999512c1ecf4500adf5f0e43
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personInterest = {
  categories: [
    "categories-value"
  ],
  description: "description-value",
  displayName: "displayName-value",
  webUrl: "webUrl-value"
};

let res = await client.api('/me/profile/interests')
    .version('beta')
    .post(personInterest);

```