---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 05f45e812cffaeeb2dda2b89cbd0f9c3f691b8b1606620c91b8e105927fc87b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57210406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let entitlementManagementSettings = await client.api('/identityGovernance/entitlementManagement/settings')
    .version('beta')
    .get();

```