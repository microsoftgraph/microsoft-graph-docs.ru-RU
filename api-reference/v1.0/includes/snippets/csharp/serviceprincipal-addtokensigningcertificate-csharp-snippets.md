---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ca463d9efba5b515444a996a4af5d8d40dc734e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "CN=customDisplayName";

var endDateTime = DateTimeOffset.Parse("2024-01-25T00:00:00Z");

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .AddTokenSigningCertificate(displayName,endDateTime)
    .Request()
    .PostAsync();

```