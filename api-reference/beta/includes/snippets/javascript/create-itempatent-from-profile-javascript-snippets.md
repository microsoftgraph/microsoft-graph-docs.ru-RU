---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 05c4391c7e7111dc6089fff0bb61bb0612a81d48
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPatent = {
  description: 'Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.',
  displayName: 'Inferring User Intent through browsing behaviors',
  isPending: true,
  number: 'USPTO-3954432633',
  webUrl: 'https://patents.gov/3954432633'
};

await client.api('/me/profile/patents')
    .version('beta')
    .post(itemPatent);

```