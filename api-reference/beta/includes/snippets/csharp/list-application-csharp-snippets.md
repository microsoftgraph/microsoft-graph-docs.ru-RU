---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: be5a5c523727e3ad0b162f4aba5f1c2647ee8486
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.Applications
    .Request()
    .GetAsync();

```