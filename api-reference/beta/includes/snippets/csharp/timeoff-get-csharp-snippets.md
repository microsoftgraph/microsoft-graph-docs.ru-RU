---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb5fe6ac188762ffe0ceae73c6b69bc827b0e1be
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOff = await graphClient.Teams["{teamId}"].Schedule.TimesOff["{timeOffId}"]
    .Request()
    .GetAsync();

```