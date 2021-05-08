---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fb082f2704394127252cd80ed62fb3458293cd5c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAsset = new Microsoft.Graph.WindowsUpdates.UpdatableAssetGroup
{
};

await graphClient.Admin.Windows.Updates.UpdatableAssets
    .Request()
    .AddAsync(updatableAsset);

```