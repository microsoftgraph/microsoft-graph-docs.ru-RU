---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 23845df05d57f783ffe0df8c2e31ac11dbbdb5549e7d94fa26d8f75e850f9dfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  'members@odata.bind': [
    'https://graph.microsoft.com/v1.0/directoryObjects/{id}',
    'https://graph.microsoft.com/v1.0/directoryObjects/{id}',
    'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
    ]
};

await client.api('/groups/{group-id}')
    .update(group);

```