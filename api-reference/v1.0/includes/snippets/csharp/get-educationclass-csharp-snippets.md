---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 576455c14e1235b36842631d076f0d76aac5eefd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["{class-id}"]
    .Request()
    .GetAsync();

```