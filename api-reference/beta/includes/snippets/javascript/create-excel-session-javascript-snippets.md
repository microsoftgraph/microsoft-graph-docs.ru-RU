---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ea487b7587515bffa9662b4cdad27cee28fb8078
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookSessionInfo = {
  persistChanges: true
};

let res = await client.api('/me/drive/items/{id}/workbook/createSession')
    .version('beta')
    .post(workbookSessionInfo);

```