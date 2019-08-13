---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 638945d7b719da3de38a6d687b5f85a358b48c84
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359278"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityMinuteCounts = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```