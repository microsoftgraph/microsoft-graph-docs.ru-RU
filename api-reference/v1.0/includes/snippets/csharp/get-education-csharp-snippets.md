---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 71c5a2f00fd028a19c63c16653f80ab77d624582
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRoot = await graphClient.Education
    .Request()
    .GetAsync();

```