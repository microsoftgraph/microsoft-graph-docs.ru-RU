---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c6a4706c8bba123196be33eaa1ada98853f94f6c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954266"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageSummariesByUser = await graphClient.Print.Reports.MonthlyPrintUsageSummariesByUser
    .Request()
    .GetAsync();

```