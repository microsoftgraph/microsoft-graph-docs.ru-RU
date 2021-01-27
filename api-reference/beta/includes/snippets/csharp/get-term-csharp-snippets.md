---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce4e3a0791512505e9685e6a50d210be41bfcf85
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = await graphClient.TermStore.Groups["{groupId}"].Sets["{setId}"].Terms["{termId}"]
    .Request()
    .GetAsync();

```