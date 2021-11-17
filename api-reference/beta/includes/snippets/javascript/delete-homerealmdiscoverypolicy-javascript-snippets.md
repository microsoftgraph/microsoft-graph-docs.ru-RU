---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 229f45cdc9e8b3c7e9a626ec996e75ab82cf3dc8197d5e2cf404adf395ac982f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57253000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .version('beta')
    .delete();

```