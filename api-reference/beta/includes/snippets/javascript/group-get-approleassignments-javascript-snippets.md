---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d55e8a8ab347ef0c48b050bbe6a215d667d38e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments')
    .version('beta')
    .get();

```