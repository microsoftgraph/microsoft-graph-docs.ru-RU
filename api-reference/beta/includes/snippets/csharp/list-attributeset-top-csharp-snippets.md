---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0f17582e12228562d7c66b69dab8d57a5451cc78
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attributeSets = await graphClient.Directory.AttributeSets
    .Request()
    .Top(10)
    .GetAsync();

```