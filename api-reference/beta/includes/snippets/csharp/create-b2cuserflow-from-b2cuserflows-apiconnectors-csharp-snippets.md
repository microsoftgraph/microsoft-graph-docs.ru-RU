---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49beb30056eae8853d5302a544a92e4992ecee5d
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51613488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = new B2cIdentityUserFlow
{
    Id = "UserFlowWithAPIConnector",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f,
    ApiConnectorConfiguration = new UserFlowApiConnectorConfiguration
    {
        PostFederationSignup = new IdentityApiConnector
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.id", "{apiConnectorId}"}
            }
        },
        PostAttributeCollection = new IdentityApiConnector
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.id", "{apiConnectorId}"}
            }
        }
    }
};

await graphClient.Identity.B2cUserFlows
    .Request()
    .AddAsync(b2cIdentityUserFlow);

```