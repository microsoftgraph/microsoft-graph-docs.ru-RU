---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9def089aee952851c50f7f3ff579096029edcebd46c4e51c1846c2df4b19b71d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050934"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const adminConsentRequestPolicy = {
  isEnabled: true,
  notifyReviewers: true,
  remindersEnabled: true,
  requestDurationInDays: 5,
  reviewers: [
    {
      query: '/users/b6879be8-fb87-4482-a72e-18445d2b5c54',
      queryType: 'MicrosoftGraph'
    },
    {
      query: '/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9',
      queryType: 'MicrosoftGraph'
    }
  ]
};

await client.api('/policies/adminConsentRequestPolicy')
    .version('beta')
    .put(adminConsentRequestPolicy);

```