---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: be0f83064a3f297e8efa9f80f3337d122b86981e2a4392fc6120725f21b356c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackage = new AccessPackage
{
    DisplayName = "Access Package New Name"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"]
    .Request()
    .UpdateAsync(accessPackage);

```