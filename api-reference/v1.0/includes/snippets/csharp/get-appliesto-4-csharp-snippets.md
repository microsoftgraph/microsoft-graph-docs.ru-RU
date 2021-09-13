---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4315b7de1f2394f269b29a4f9dfd8a2855516ec4af4291a9a948ab196b9a39bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57370665"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.TokenLifetimePolicies["{tokenLifetimePolicy-id}"].AppliesTo
    .Request()
    .GetAsync();

```