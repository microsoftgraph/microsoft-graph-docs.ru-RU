---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a6fca3a97bba5b7d89b7b77c9b5581ae75a2198
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appManagementPolicies = await client.api('/policies/appManagementPolicies')
    .version('beta')
    .get();

```