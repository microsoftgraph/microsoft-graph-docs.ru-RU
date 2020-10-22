---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46bac48b55847d9304d330a60af8490481bb7f8c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "edit",
  scope: "organization"
};

let res = await client.api('/me/drive/items/{item-id}/createLink')
    .post(permission);

```