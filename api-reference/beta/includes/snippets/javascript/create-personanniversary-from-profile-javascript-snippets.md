---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f6607b272f77aec6ea3ec17ad1ade0f384b94589
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnualEvent = {
  type: 'birthday',
  date: '1980-01-08'
};

await client.api('/me/profile/anniversaries')
    .version('beta')
    .post(personAnnualEvent);

```