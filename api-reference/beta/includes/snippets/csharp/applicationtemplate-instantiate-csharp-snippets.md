---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1717a8034ee70798bac4279d688933ed337a719
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "My custom name";

await graphClient.ApplicationTemplates["{applicationTemplate-id}"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```