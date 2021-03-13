---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 35f99c19557c7d352edc286b34c1ae8f23fc4640
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807888"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const projectParticipation = {
  allowedAudiences: 'organization',
  client: {
    department: 'Corporate Marketing',
    webUrl: 'https://www.contoso.com'
  }
};

await client.api('/me/profile/projects/{id}')
    .version('beta')
    .update(projectParticipation);

```