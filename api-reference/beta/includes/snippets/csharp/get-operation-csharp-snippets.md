---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b741bb050e791ad54cd82f82fbbd536ba50b325
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var longRunningOperation = await graphClient.Users["{id | userPrincipalName}"].Authentication.Operations["{id}"]
    .Request()
    .GetAsync();

```