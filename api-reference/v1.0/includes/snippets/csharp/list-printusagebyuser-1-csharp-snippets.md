---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 15ba3d457a7d649ade5e9ca37d44166633234025d56c1996141786a892b443ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57268390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByUser = await graphClient.Reports.DailyPrintUsageByUser
    .Request()
    .GetAsync();

```