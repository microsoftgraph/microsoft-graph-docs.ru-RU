---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c237761df6bc7d9f0e132fde15b551d0668f221
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{directoryObject-id}"]
    .Request()
    .Filter("isOf('Microsoft.Graph.User') or isOf('Microsoft.Graph.Group')")
    .GetAsync();

```