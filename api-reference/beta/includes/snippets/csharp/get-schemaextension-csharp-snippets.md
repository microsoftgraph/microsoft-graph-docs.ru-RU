---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3f21fe4aa3646cdac9f1b2e1f3a7a9b0fc10478a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = await graphClient.SchemaExtensions["graphlearn_test"]
    .Request()
    .GetAsync();

```