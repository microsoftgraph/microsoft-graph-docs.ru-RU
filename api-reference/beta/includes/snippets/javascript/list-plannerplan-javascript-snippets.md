---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a6400fc54ad13736ebe67b98c4e59ecad030acfb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rosterPlans = await client.api('/users/{usersId}/planner/rosterPlans')
    .version('beta')
    .get();

```