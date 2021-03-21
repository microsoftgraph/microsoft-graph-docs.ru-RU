---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7df4a487d16d9ea6519f26a936de221c7d315075
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962211"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.ServicePrincipals["{servicePrincipal-id}"].OwnedObjects
    .Request()
    .GetAsync();

```