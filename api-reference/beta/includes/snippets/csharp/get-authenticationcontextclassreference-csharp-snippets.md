---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: be5d30ce8deb9c3f8edf891d6de0073d0a776352
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationContextClassReferences = await graphClient.Identity.ConditionalAccess.AuthenticationContextClassReferences
    .Request()
    .GetAsync();

```