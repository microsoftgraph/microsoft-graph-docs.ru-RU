---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0efd2090a332b0e70805427afe552a756bb71d88
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let audioRoutingGroups = await client.api('/communications/calls/{id}/audioRoutingGroups')
    .version('beta')
    .get();

```