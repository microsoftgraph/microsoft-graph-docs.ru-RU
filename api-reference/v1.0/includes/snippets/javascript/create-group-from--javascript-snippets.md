---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b6584f8c8328868fcbf75d1ee54a5977178e6fc8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/groups/{groupId}'
};

await client.api('/print/shares/{printerShareId}/allowedGroups/$ref')
    .post(group);

```