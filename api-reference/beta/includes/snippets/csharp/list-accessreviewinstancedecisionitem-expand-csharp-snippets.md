---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ada4b07386af4fa5076ac7a6996c9e3317fafbf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332871"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Decisions
    .FilterByCurrentUser(AccessReviewInstanceDecisionItemFilterByCurrentUserOptions.Reviewer)
    .Request()
    .Expand("instance($expand=definition)")
    .GetAsync();

```