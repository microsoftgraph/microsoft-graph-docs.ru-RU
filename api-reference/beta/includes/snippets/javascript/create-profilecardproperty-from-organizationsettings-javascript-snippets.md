---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 168160ef4a02db31961f62c7d605cf8159b1232f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profileCardProperty = {
  directoryPropertyName: 'CustomAttribute1',
  annotations: [
    {
      displayName: 'Cost Center',
      localizations: [
        {
          languageTag: 'ru-RU',
          displayName: 'центр затрат'
        }
      ]
    }
  ]
};

await client.api('/organization/{organizationId}/settings/profileCardProperties')
    .version('beta')
    .post(profileCardProperty);

```