---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f9644e89c477a36eb65bc3297dac73c4b57e0147
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registrants = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.Registrants
    .Request()
    .GetAsync();

```