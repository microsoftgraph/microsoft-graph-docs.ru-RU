---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7f20f3879b09b9d9d5f47cc7ac3524fa4c12ec50
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "37429217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

let res = await client.api('/directoryObjects/{object-id}/getMemberGroups')
    .post(string);

```