---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a2b7ab66bd694059c11ad1a869d27578c2065d9a
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemActivityStat = await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Analytics.AllTime
    .Request()
    .GetAsync();

```