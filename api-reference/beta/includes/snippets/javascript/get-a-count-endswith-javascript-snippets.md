---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aef6b78eb1c3df6c0a52f5aa8d8ebac66e67a983
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('endswith(mail,\'a@contoso.com\')')
    .orderby('userPrincipalName')
    .get();

```