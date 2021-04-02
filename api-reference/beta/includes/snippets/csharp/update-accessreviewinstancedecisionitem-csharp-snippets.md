---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e843c20489eaf390de57b7ce058561bf226e6019
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem
{
    Decision = "Approve",
    Justification = "This person is still on my team"
};

await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"].Decisions["{accessReviewInstanceDecisionItem-id}"]
    .Request()
    .UpdateAsync(accessReviewInstanceDecisionItem);

```