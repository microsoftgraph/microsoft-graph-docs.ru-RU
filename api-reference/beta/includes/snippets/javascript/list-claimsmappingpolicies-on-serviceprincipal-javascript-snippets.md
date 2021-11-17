---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79b6a56c56ced59f0da2382f10fbfb277429c2768abe727d0a274834dea16fb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57247117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicies = await client.api('/servicePrincipals/{id}/claimsMappingPolicies')
    .version('beta')
    .get();

```