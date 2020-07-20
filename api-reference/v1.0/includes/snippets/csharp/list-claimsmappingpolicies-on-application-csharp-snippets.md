---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bf49a45e64765614cdfb34209f065ea96a4bafb8
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicies = await graphClient.ServicePrincipals["{id}"].ClaimsMappingPolicies
    .Request()
    .GetAsync();

```