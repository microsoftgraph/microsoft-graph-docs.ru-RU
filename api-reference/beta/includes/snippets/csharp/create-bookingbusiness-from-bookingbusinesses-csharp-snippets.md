---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18fa828e25991bbb5f7d1eee15074273fade0e81
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65947049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = new BookingBusiness
{
    DisplayName = "Fourth Coffee",
    Address = new PhysicalAddress
    {
        PostOfficeBox = "P.O. Box 123",
        Street = "4567 Main Street",
        City = "Buffalo",
        State = "NY",
        CountryOrRegion = "USA",
        PostalCode = "98052"
    },
    Phone = "206-555-0100",
    Email = "manager@fourthcoffee.com",
    WebSiteUrl = "https://www.fourthcoffee.com",
    DefaultCurrencyIso = "USD"
};

await graphClient.BookingBusinesses
    .Request()
    .AddAsync(bookingBusiness);

```