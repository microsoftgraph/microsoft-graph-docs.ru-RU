---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 937ca44aa88325d490bed4187b88b3c5cb416868d177fa2c8f0f08916e36f453
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57397031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments["{identityUserFlowAttributeAssignment-id}"]
    .Request()
    .GetAsync();

```