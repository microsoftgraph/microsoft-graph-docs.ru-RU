---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1d592a63a4876e6220ef8b514cb38874e230708a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.TrustFramework.Policies
    .Request()
    .GetAsync();

```