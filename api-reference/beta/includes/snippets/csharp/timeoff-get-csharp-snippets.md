---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9688aeed9a3c4641b82b606c2a695319c681a954
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOff = await graphClient.Teams["{team-id}"].Schedule.TimesOff["{timeOff-id}"]
    .Request()
    .GetAsync();

```