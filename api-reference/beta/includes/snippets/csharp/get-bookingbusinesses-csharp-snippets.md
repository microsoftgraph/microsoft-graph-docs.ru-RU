---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6ac0e2391255a63614ff7948d9f6c1b7a83aefa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusinesses = await graphClient.BookingBusinesses
    .Request()
    .GetAsync();

```