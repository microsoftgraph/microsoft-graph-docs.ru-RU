---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8481e51a1c87aa8919ff4e9824f1251cef78d911
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyServicePrincipal = await graphClient.IdentityProtection.RiskyServicePrincipals["{riskyServicePrincipal-id}"]
    .Request()
    .GetAsync();

```