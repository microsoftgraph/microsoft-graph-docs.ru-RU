---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06555861673234ca830051fb6567938919858585
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = new PrintConnector
{
    Name = "ConnectorName",
    FullyQualifiedDomainName = "CONNECTOR-MACHINE",
    OperatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
    AppVersion = "0.19.7338.23496",
    Location = new PrinterLocation
    {
        Latitude = 1.1,
        Longitude = 2.2,
        AltitudeInMeters = 3
    }
};

await graphClient.Print.Connectors["{printConnector-id}"]
    .Request()
    .UpdateAsync(printConnector);

```