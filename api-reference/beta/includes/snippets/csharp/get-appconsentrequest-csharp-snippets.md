---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c74d7f9091bae89f30c736cf1fbc6b894f898f2792330abe917aa2bb27183ce5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appConsentRequest = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"]
    .Request()
    .GetAsync();

```