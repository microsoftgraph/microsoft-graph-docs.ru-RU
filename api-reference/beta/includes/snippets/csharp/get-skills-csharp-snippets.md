---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b28b6d3eed5a2db857233efe422503da8d2492ab
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skills = await graphClient.Me.Profile.Skills
    .Request()
    .GetAsync();

```