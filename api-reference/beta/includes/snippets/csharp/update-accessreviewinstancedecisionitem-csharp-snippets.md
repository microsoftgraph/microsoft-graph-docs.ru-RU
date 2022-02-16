---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ee862f8fd9e96c063ea2692086a750e2a17bd4e
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62855792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem
{
    Decision = "Approve",
    Justification = "This person is still on my team"
};

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Stages["{accessReviewStage-id}"].Decisions["{accessReviewInstanceDecisionItem-id}"]
    .Request()
    .UpdateAsync(accessReviewInstanceDecisionItem);

```