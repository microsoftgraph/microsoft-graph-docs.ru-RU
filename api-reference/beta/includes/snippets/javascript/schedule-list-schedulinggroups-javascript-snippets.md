---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f8512e16a53789572f8bed0c1a6f40a644781ad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedulingGroups = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .version('beta')
    .get();

```