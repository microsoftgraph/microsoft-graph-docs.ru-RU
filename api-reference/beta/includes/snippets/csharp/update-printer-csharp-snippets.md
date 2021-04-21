---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 628cb7b3b24f23dd4745d8ab9efe0608041af413
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = new Printer
{
    Name = "PrinterName",
    Location = new PrinterLocation
    {
        Latitude = 1.1,
        Longitude = 2.2,
        AltitudeInMeters = 3
    }
};

await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .UpdateAsync(printer);

```