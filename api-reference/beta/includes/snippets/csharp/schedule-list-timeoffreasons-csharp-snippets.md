---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 57c30fcdd64927a5301f20041b26941b6aa233dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809416"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReasons = await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons
    .Request()
    .GetAsync();

```