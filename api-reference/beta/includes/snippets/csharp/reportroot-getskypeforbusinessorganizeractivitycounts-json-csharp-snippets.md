---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07cbb46556b096a66c2ba512cc0b34d803998895
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359377"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityCounts("D7")
    .Request()
    .GetAsync();

```