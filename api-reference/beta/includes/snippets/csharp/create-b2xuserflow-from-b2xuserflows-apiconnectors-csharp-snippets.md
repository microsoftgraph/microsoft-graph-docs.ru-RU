---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bbf1b095c3661cd58cfc5c95c5ffe8e64ae4cf88
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = new B2xIdentityUserFlow
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

await graphClient.Identity.B2xUserFlows
    .Request()
    .AddAsync(b2xIdentityUserFlow);

```