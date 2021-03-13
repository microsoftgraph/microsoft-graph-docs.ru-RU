---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 282a9f170a5805421d1fc44653ad25fdd08769f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783284"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let favoritePlans = await client.api('/me/planner/favoritePlans')
    .version('beta')
    .get();

```