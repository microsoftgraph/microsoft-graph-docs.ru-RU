---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ed19155fd4712fe0f2faacb26c754a17353f3122c5c9dfe8743fe428417959d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["{educationUser-id}"]
    .Request()
    .GetAsync();

```