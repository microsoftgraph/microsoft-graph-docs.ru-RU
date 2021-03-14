---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bdbcb882c618bf89d9c370617b491754f12f4cef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .delete();

```