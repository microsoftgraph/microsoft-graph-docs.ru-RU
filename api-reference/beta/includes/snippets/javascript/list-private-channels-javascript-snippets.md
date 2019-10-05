---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa74332b562ded029cb98cc2c16f69b2c6d035f2
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .version('beta')
    .filter('membershipType eq 'private'')
    .get();

```