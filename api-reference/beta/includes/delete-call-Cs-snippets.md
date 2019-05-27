---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 881ec7bac57269dbf90029c04bc7ea76988cf56c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["{id}"]
    .Request()
    .DeleteAsync();

```