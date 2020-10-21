---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 71c5a2f00fd028a19c63c16653f80ab77d624582
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRoot = await graphClient.Education
    .Request()
    .GetAsync();

```