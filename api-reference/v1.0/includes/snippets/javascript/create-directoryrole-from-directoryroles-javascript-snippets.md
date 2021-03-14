---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bf1dbc487d0bf0689348cc86acc8ed0cf3bd87ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  roleTemplateId: 'roleTemplateId-value'
};

await client.api('/directoryRoles')
    .post(directoryRole);

```