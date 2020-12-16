---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0037d172b23d9bc5643d4955cd9249588e5abc24
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689271"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentOrder = await graphClient.Identity.B2cUserFlows["{id}"].UserAttributeAssignments
    .GetOrder()
    .Request()
    .GetAsync();

```