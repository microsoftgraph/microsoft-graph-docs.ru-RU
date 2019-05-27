---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 090b9ad328a4fcf3653448ce3a69330a28a6a1cd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programs = await graphClient.Programs
    .Request()
    .GetAsync();

```