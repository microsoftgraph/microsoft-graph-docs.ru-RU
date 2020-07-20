---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a0a9d95267fa6a9fbe2d1c9246f561e9b839a79e
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationFlowsPolicy = await graphClient.Policies.AuthenticationFlowsPolicy
    .Request()
    .GetAsync();

```