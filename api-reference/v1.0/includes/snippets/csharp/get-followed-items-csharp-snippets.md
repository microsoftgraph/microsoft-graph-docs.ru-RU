---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 006bd9316b777233b585673243deff7d9e292bc7
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var following = await graphClient.Me.Drive.Following
    .Request()
    .GetAsync();

```