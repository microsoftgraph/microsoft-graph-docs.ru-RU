---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f69b5f40588f6881e65fe625ca7d1505ee39b73c32caec7ae4ab4e937c3e8adb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const skillProficiency = {
  categories: [
    'Professional'
  ],
  allowedAudiences: 'organization',
  displayName: 'API Design',
  proficiency: 'generalProfessional',
  collaborationTags: [
    'ableToMentor'
  ]
};

await client.api('/me/profile/skills')
    .version('beta')
    .post(skillProficiency);

```