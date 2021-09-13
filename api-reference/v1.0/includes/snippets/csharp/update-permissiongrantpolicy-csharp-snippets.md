---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2bce7e329a7b7af1166643e48d2646ef13ee6cdf3175a2a0221f0ad2273677dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = new PermissionGrantPolicy
{
    DisplayName = "Custom permission grant policy"
};

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"]
    .Request()
    .UpdateAsync(permissionGrantPolicy);

```