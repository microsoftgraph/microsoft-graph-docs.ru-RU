---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e48f954eee39c4345ef25ed01fb2624775bf943d96905940037b3579e0af25c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57432133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .filter('identities/any(c:c/issuerAssignedId eq \'j.smith@yahoo.com\' and c/issuer eq \'contoso.onmicrosoft.com\')')
    .select('displayName,id')
    .get();

```