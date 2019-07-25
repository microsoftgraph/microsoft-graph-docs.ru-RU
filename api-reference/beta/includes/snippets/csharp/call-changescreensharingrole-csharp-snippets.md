---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 734e9bcfe77c82f5e67e9903567314dcea0a4da3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708989"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var role = ScreenSharingRole.Viewer;

await graphClient.App.Calls["{id}"]
    .ChangeScreenSharingRole(role)
    .Request()
    .PostAsync();

```