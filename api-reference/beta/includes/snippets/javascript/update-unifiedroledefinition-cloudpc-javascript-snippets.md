---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e8e62782ac64a1a8e1e4e98835ba80f586571752
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleDefinition = {
  description: 'Update basic properties and permission of application registrations',
  displayName: 'ExampleCustomRole',
  rolePermissions: 
    [
        {
            allowedResourceActions: 
            [
                'Microsoft.CloudPC/CloudPCs/Read',
                'Microsoft.CloudPC/CloudPCs/Reprovision'
            ]
        }
    ]
};

await client.api('/roleManagement/cloudPc/roleDefinitions/b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff')
    .version('beta')
    .update(unifiedRoleDefinition);

```