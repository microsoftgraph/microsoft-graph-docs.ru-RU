---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6257bc6eec807e70970882861012d60510488355cfa5d8b7915647895eacf23b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57307963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skills = await graphClient.Me.Profile.Skills
    .Request()
    .GetAsync();

```