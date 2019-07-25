---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d53f3fafdda4da97e14e9a2e4ca84a2527a67895
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var staffMembers = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers
    .Request()
    .GetAsync();

```