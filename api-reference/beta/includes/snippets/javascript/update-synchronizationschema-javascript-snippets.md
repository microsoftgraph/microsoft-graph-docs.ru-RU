---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 34f3cc862a7c348c9297171258c85a174905cf20
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationSchema = {
    directories: [
        {
            name: "Azure Active Directory",
            objects: [
                {
                    name: "User",
                    attributes: [
                        {
                            name: "userPrincipalName",
                            type: "string"
                        }
                    ]
                },
            ]
        },
        {
            name: "Salesforce",
        }
    ],
    synchronizationRules:[
        {
            name: "USER_TO_USER",
            sourceDirectoryName: "Azure Active Directory",
            targetDirectoryName: "Salesforce",
            objectMappings: [
                {
                    sourceObjectName: "User",
                    targetObjectName: "User",
                    attributeMappings: [
                        {
                            source: {},
                            targetAttributeName: "userName"
                        },
                    ]
                },
            ]
        },
    ]
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .put({synchronizationSchema : synchronizationSchema});

```