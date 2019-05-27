---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6f1a2651a6c7319c8f8cabe9c26511ede97d2ab
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .DeleteAsync();

```