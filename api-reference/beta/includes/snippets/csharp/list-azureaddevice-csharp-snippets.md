---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ecfa2b890052c4e2aba61536144859a0d82f186928a539e2e09799a47584cbce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57371426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAssets = await graphClient.Admin.Windows.Updates.UpdatableAssets
    .Request()
    .Filter("isof('microsoft.graph.windowsUpdates.azureADDevice')")
    .GetAsync();

```