---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b3a5a9f788ef181bb429abf3c13b587307186e4bd0267d8ec70a31cd579d8fd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57191017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decision = "Approve";

var justification = "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team";

var resourceId = "a5c51e59-3fcd-4a37-87a1-835c0c21488a";

await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"]
    .BatchRecordDecisions(decision,justification,null,resourceId)
    .Request()
    .PostAsync();

```