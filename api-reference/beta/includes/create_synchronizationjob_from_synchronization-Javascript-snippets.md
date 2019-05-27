---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eb125b9b027cdb5d3f27765065301830317cb82e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationJob = {
    templateId: "BoxOutDelta"
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs')
    .version('beta')
    .post({synchronizationJob : synchronizationJob});

```