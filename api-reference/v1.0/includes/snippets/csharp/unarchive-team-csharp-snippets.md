---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 407be1873b6cf760d95a0fe7c1f325f3379ce277
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"]
    .Unarchive()
    .Request()
    .PostAsync();

```