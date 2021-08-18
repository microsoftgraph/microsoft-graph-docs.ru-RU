---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 77b0f7e89738ffc78069a9121dab24ceb721bffc
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Groups["{group-id}"].Members
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Pr")
    .Select("displayName,id")
    .OrderBy("displayName")
    .GetAsync();

```