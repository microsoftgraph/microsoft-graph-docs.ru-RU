---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b6b353d82ea072ad6b6680bd9cc0b34e3cbafac5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.IdentityProviders
    .Request()
    .GetAsync();

```