---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92af74ff7f8105926f631ef71f826c8fe3e4321b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: [ "read" ]
};

let res = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .update({permission : permission});

```