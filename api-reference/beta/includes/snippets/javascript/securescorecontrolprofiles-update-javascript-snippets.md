---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3f59e5537c413e2dd0117eb3350564f55349fec8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504829"
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
    .update({secureScoreControlProfile : secureScoreControlProfile});

```