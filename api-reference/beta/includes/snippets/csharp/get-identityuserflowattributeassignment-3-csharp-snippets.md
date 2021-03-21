---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e2a11772daef8807aee124cac260391bd2a1a76e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserAttributeAssignments["{identityUserFlowAttributeAssignment-id}"]
    .Request()
    .GetAsync();

```