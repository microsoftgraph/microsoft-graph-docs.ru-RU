---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e45e468f89c2608bb6dfe3e07c4fe8f801617e2a01c09b4ab1f5d9c98593df1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57251989"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.ServicePrincipals["{servicePrincipal-id}"].OwnedObjects
    .Request()
    .GetAsync();

```