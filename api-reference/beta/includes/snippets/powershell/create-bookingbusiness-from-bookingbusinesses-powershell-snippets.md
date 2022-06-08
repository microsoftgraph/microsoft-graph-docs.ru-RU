---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9755eb04c80fa58a3049688e0af8d20301a5399e
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65947046"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    DisplayName = "Fourth Coffee"
    Address = @{
        PostOfficeBox = "P.O. Box 123"
        Street = "4567 Main Street"
        City = "Buffalo"
        State = "NY"
        CountryOrRegion = "USA"
        PostalCode = "98052"
    }
    Phone = "206-555-0100"
    Email = "manager@fourthcoffee.com"
    WebSiteUrl = "https://www.fourthcoffee.com"
    DefaultCurrencyIso = "USD"
}

New-MgBookingBusiness -BodyParameter $params

```