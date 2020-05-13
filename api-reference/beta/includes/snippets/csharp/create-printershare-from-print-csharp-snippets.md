---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2841bf8612b8fc1cfcadd6070eb7bd8a34df52b8
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    Name = "name-value",
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind","https://graph.microsoft.com/beta/print/printers/{id}"}
    }
};

await graphClient.Print.Shares
    .Request()
    .AddAsync(printerShare);

```