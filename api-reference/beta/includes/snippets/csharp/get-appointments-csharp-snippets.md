---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc676f1a254a4654cbc4ea3b155877fbb6f5bc48
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appointments = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments
    .Request()
    .GetAsync();

```