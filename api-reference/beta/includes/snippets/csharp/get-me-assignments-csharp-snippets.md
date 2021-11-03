---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ded67cfc806d675c0caca8c72ec103cb4a2c445d
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Me.Assignments
    .Request()
    .GetAsync();

```