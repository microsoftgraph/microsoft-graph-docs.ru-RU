---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0c5f1c63824866ebc5f21d35212a70b279bbf6e4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210468"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "785f4929-92ca-497b-863f-c778c77c9758";

await graphClient.Communications.Calls["{call-id}"]
    .AddLargeGalleryView(clientContext)
    .Request()
    .PostAsync();

```