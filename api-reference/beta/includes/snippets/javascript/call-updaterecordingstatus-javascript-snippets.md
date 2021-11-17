---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 583fb1ceba17b79de9aa73ec5e3eee16934f79f64dba32bf857a8185e50ccb90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateRecordingStatusOperation = {
  clientContext: 'clientContext-value',
  status: 'notRecording | recording | failed'
};

await client.api('/communications/calls/{id}/updateRecordingStatus')
    .version('beta')
    .post(updateRecordingStatusOperation);

```