---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d5b58472824f38cf31a4f3358803f12692fdc82c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    DisplayName = "PrinterShare Name",
    AllowAllUsers = false,
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind", "https://graph.microsoft.com/v1.0/print/printers/{printerId}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .UpdateAsync(printerShare);

```