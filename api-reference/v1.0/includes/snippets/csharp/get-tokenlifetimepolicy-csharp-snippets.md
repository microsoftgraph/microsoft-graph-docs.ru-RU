---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a5aeea03004d95f75903c5bb9a4789525d7ad6a66da605c9c28f8d01bcf64e81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = await graphClient.Policies.TokenLifetimePolicies["{tokenLifetimePolicy-id}"]
    .Request()
    .GetAsync();

```