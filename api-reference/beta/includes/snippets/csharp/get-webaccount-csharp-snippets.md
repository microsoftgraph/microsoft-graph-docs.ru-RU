---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e464cbcb7e24fdd173a6d43decc5582fb2819c3
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = await graphClient.Me.Profile.WebAccounts["{id}"]
    .Request()
    .GetAsync();

```