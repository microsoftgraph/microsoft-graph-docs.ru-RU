---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fbb299faab47eeebddbeb235ea98217e35d68e37
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: 'String',
  closedDateTime: 'String (timestamp)',
  comments: ['String'],
  feedback: '@odata.type: microsoft.graph.alertFeedback',
  status: '@odata.type: microsoft.graph.alertStatus',
  tags: ['String'],
  vendorInformation: 
    {
      provider: 'String',
      vendor: 'String'
    }
};

await client.api('/security/alerts/{alert_id}')
    .version('beta')
    .update(alert);

```