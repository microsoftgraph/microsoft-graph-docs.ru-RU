---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b0d62038430008c7d73aaf07827b2d5e7a2eb85
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956669"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Classes
    .Request()
    .GetAsync();

```