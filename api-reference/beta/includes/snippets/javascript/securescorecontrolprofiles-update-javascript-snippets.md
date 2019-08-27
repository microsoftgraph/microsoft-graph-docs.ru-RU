---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b0109c81f00bd44ccab9cfd58be24976e0dd612f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const secureScoreControlProfile = {
  controlStateUpdates: "controlStateUpdates-value"
};

let res = await client.api('/security/secureScoreControlProfiles/AdminMFA')
    .version('beta')
    .update(secureScoreControlProfile);

```