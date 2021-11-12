---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 696fd62cfce58a21ff5a1916ca358b1cc64f6807cf2c8f707345a152b0ecf3d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57373095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTaskTrigger = {
  event: 'jobStarted',
  'definition@odata.bind': 'https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}'
};

await client.api('/print/printers/{printerId}/taskTriggers')
    .post(printTaskTrigger);

```