---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 315147aa73d359325d0fbfb8db33303ba0b43d75ad9fd3dfe0101e2befcf15b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57268168"
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