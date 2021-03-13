---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 553ffd0e651788f89e0e1cc28eacf2c5a5549fbb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let audioRoutingGroup = await client.api('/communications/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .get();

```