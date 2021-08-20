---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 553987912ea90137d90373ea24ca942286bf848707379d0e52d5e0d8f8cbf85b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Team')
    .get();

```