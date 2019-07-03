---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d1d4212611a535f0d014a6fc7f6bf6c7cf2bb935
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageVersionsUserCounts = await graphClient.Reports.GetEmailAppUsageVersionsUserCounts('D7')
    .Request()
    .GetAsync();

```