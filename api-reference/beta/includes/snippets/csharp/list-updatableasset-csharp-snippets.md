---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b90332d6a081be6e5e333d199898d1a53174c83c
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52476689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var exclusions = await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"].Audience.Exclusions
    .Request()
    .GetAsync();

```