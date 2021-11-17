---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1e90830447b475cbe9b26ec571b3eb4f10cb43bf1c9bd751e0f634200b4f4b0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrantPolicies = await client.api('/policies/permissionGrantPolicies')
    .version('beta')
    .get();

```