---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44d00c7a706c3dabc1ea8b75126bc8f3cfc1d318
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplates = await graphClient.GroupSettingTemplates
    .Request()
    .GetAsync();

```