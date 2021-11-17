---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1c0f9fefc6e8b7fd56efaf9977c7355495cb75abd46c44912cdf8ceaa4e2663c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"].Decisions
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```