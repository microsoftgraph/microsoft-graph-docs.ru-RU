---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 090b9ad328a4fcf3653448ce3a69330a28a6a1cd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programs = await graphClient.Programs
    .Request()
    .GetAsync();

```