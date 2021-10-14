---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ea77ec212a1212c0834feb65c35ebd9a9184f32bc32d60b392af4955217bc61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignedTo["{appRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```