---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a68851b68996c90b50c2b00856ab2d7c6dab0d94
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleSetting = {
   adminEligibleSettings:[
      {
         ruleIdentifier:"ExpirationRule",
         setting:{\"permanentAssignment\:false,\maximumGrantPeriodInMinutes\:129600}"
      }
   ]
};

let res = await client.api('/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5')
    .version('beta')
    .update({governanceRoleSetting : governanceRoleSetting});

```