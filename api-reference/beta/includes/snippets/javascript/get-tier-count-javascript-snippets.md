---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e663152c7be37b88c4f84a4ccc672829e680cd15252aeae05ab50f454143fad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57254429"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/groups/{id}/transitiveMembers/microsoft.graph.user')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:tier')
    .select('displayName,id')
    .orderby('displayName')
    .get();

```