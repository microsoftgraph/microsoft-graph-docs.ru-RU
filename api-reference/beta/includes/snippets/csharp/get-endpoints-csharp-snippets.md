---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d7facad907a2aca09440340b459e6625cf28b58
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reportRoot = await graphClient.Print.Reports["monthlyPrintUsageSummariesByPrinter"]
    .Request()
    .GetAsync();

```