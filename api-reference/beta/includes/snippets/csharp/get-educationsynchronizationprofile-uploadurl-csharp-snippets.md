---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c1bed413504ae398a38ddaa749520c26f13cb185
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786379"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .UploadUrl()
    .Request()
    .GetAsync();

```