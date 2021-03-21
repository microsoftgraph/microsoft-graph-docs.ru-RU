---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f4e2b6b107a2677d3b9da660266c15a3c89b13f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959820"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/homeRealmDiscoveryPolicies/{id}/appliesTo')
    .get();

```