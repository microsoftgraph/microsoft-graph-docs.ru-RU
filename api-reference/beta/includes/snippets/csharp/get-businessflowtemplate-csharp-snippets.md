---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc280236aa5170886c5f2778f31214bf72cc0264
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var businessFlowTemplates = await graphClient.BusinessFlowTemplates
    .Request()
    .GetAsync();

```