---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5854f06d1121d95a868de8cfdda016f8599247f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoleTemplates = await client.api('/directoryRoleTemplates')
    .version('beta')
    .get();

```