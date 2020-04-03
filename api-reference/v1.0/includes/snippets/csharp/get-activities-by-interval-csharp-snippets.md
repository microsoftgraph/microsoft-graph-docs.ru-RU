---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 542de2a57a3a9fe1430419ddcaaf58087dafe99f
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getActivitiesByInterval = await graphClient.Drives["{drive-id}"].Items["{item-id}"]
    .GetActivitiesByInterval("2017-01-01","2017-01-3","day")
    .Request()
    .GetAsync();

```