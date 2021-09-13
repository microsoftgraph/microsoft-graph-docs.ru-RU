---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e7d2689d7ca0b7bbeba981f31d88952af644923747dc5cfc736935c3acc86618
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userConsentRequests = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests
    .Request()
    .GetAsync();

```