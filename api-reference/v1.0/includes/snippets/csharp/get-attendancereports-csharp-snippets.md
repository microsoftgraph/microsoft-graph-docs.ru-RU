---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ec0abf1f49b6811f983dda5f078c82fe07eb63d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attendanceReports = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendanceReports
    .Request()
    .GetAsync();

```