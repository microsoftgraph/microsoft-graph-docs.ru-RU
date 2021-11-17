---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1ef5d6bf8f3e2a5dba45159085853bd87e799300c0dd68844d93180c9d24db3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256049"
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