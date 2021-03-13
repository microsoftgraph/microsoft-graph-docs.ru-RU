---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e75aa5954ea6f16df74678766930beba92fe552
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const secureScoreControlProfile = {
  controlStateUpdates: 'controlStateUpdates-value'
};

await client.api('/security/secureScoreControlProfiles/AdminMFA')
    .version('beta')
    .update(secureScoreControlProfile);

```