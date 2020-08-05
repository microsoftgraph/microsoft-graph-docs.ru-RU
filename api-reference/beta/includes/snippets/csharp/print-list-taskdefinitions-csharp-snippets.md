---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0ec52b5288291ea748b8cf07aaaf715c6e905f62
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskDefinitions = await graphClient.Print.TaskDefinitions
    .Request()
    .GetAsync();

```