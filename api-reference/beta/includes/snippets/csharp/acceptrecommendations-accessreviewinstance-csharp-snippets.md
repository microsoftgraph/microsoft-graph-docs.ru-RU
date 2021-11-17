---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0aa59e85eb416bd002ad1af00e6d9a72648e0e91d3c3f1feefecd22f5d538ff5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"]
    .AcceptRecommendations()
    .Request()
    .PostAsync();

```