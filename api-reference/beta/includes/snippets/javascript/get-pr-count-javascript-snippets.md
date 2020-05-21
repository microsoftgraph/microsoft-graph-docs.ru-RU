---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 32d9bd56f36293520bf09dc05a0b98ca8c27c180
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members/microsoft.graph.user')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Pr')
    .select('displayName,id')
    .orderby('displayName ')
    .get();

```