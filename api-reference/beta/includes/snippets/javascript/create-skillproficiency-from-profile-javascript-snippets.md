---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 77ef105785e12bf1a673b9d067bcbbcaaf0c6256
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808964"
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