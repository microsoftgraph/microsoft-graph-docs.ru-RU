---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d1b33c7a2ee92b75ade5703eb3bd32d95f79968e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60718491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const continuousAccessEvaluationPolicy = {
  '@odata.type': '#microsoft.graph.continuousAccessEvaluationPolicy',
  migrate: true
};

await client.api('/identity/continuousAccessEvaluationPolicy')
    .version('beta')
    .update(continuousAccessEvaluationPolicy);

```