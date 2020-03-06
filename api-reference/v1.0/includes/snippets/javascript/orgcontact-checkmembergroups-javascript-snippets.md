---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a06e76b37ba64e07ec98d1fd0bea1212ec523487
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    "groupId-value1", "groupId-value2" 
  ]
};

let res = await client.api('/contacts/{id}/checkMemberGroups')
    .post(string);

```