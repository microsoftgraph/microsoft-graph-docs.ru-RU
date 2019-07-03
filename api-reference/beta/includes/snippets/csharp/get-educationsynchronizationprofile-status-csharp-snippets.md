---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 745f9c603862d57c1da5cfd0216e3f2d595901f0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfileStatus = await graphClient.Education.SynchronizationProfiles["{id}"].ProfileStatus
    .Request()
    .GetAsync();

```