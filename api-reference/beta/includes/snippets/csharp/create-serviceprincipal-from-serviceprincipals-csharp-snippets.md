---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06faa69f714caa04de4eed3e4111ea2339f76381
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    AppId = "65415bb1-9267-4313-bbf5-ae259732ee12"
};

await graphClient.ServicePrincipals
    .Request()
    .AddAsync(servicePrincipal);

```