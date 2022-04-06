---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d17d66087b94de9d0782915acc83dfe9d39fe984
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicies = await client.api('/policies/roleManagementPolicies')
    .version('beta')
    .filter('scopeId eq \'/\' and scopeType eq \'DirectoryRole\'')
    .get();

```