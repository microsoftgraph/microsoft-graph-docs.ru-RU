---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ff5c37301921c418ae9241b1d74ba1d48063d9f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861478"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithMe = await graphClient.Me.Drive
    .SharedWithMe()
    .Request()
    .GetAsync();

```