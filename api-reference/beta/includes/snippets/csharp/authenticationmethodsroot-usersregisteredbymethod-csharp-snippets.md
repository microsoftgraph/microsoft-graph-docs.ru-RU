---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 34c2c65fb0a59e53ce4914e1871a5a6ca9a2c05f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationMethodSummary = await graphClient.Reports.AuthenticationMethods
    .UsersRegisteredByMethod(IncludedUserTypes.All,IncludedUserRoles.All)
    .Request()
    .GetAsync();

```