---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6a6184ac5e450984570ed71b4199dfcb0e0324f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemAddress = {
  displayName: 'Home',
  detail: {
    type: 'home',
    postOfficeBox: null,
    street: '221B Baker Street',
    city: 'London',
    state: null,
    countryOrRegion: 'United Kingdom',
    postalCode: 'E14 3TD'
  }
};

await client.api('/me/profile/addresses')
    .version('beta')
    .post(itemAddress);

```