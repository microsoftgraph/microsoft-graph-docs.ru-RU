---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fcf96bcc39c1aba29bc6d95447ddb2a193aee157ab0740414543e78f48727f36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57250827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByPrinter = await graphClient.Reports.DailyPrintUsageByPrinter["{printUsageByPrinter-id}"]
    .Request()
    .GetAsync();

```