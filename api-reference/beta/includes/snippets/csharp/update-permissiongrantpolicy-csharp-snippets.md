---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 088086278820f10df34f9a214e91240ccfb17b50
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = new PermissionGrantPolicy
{
    DisplayName = "Custom permission grant policy"
};

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"]
    .Request()
    .UpdateAsync(permissionGrantPolicy);

```