---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4637ebae11553452568e67ce8f0459309585e484
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: "String",
  closedDateTime: "String (timestamp)",
  comments: [
    "String"
  ],
  feedback: "@odata.type: microsoft.graph.alertFeedback",
  status: "@odata.type: microsoft.graph.alertStatus",
  tags: [
    "String"
  ],
  vendorInformation: {
    provider: "String",
    vendor: "String"
  }
};

let res = await client.api('/security/alerts/{alert_id}')
    .update({alert : alert});

```