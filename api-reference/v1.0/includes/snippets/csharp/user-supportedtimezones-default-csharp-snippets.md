---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb4877f494f4bd4f9620268232baa74d70474948
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514684"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook.SupportedTimeZones()
    .Request()
    .GetAsync();

```