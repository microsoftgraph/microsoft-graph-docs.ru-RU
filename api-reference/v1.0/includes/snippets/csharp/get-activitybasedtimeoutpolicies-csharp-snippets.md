---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c3ad5bc09c897a39fa8a0282e63c4bfb8a82144a323def11081c740404d565a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57367114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicies = await graphClient.Policies.ActivityBasedTimeoutPolicies
    .Request()
    .GetAsync();

```