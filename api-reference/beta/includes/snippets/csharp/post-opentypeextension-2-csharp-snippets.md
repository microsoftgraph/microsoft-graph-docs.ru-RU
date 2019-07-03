---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 901f492b1c78cd27eeb055f0ab1d284042786ccc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new Extension
{
    ExtensionName = "Com.Contoso.Referral",
    CompanyName = "Wingtip Toys",
    DealValue = 500050,
    ExpirationDate = "2015-12-03T10:00:00Z"
};

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions
    .Request()
    .AddAsync(extension);

```