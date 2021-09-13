---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 583b50a658e2e563667476cf4595c091fa2e6c4016b569355a1f87457003ffe9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57206966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.Identity.ConditionalAccess.Policies
    .Request()
    .GetAsync();

```