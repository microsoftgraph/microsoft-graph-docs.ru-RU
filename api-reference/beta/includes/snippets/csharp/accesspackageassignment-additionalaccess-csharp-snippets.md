---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 597f6e9a921371ed5bbdce35e66f5c55132e24da
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var additionalAccess = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignments
    .AdditionalAccess("2506aef1-3929-4d24-a61e-7c8b83d95e6f","d5d99728-8c0b-4ede-83d2-cf9b0e8dabfb")
    .Request()
    .Expand("target")
    .GetAsync();

```