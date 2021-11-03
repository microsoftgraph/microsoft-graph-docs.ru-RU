---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc18f2495316d5283dfffe2cf482a5b249f4cf5f36a82a75d6db894c5fbccbb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')')
    .version('beta')
    .get();

```