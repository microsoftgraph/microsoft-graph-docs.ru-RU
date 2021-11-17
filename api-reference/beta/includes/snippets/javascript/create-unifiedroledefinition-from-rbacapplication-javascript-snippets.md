---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eac69d04486d9f35756c667512dc6743f4efdcf0db3de5c3f57f68f242165261
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57320844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleDefinition = {
  description: 'Update basic properties of application registrations',
  displayName: 'Application Registration Support Administrator',
  rolePermissions: 
    [
        {
            allowedResourceActions: 
            [
                'microsoft.directory/applications/basic/read'
            ]
        }
    ],
    isEnabled: 'true'
};

await client.api('/roleManagement/directory/roleDefinitions')
    .version('beta')
    .post(unifiedRoleDefinition);

```