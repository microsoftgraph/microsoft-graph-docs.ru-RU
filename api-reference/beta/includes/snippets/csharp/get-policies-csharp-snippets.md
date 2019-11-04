---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 324cf49890987c135d028c5d13f51bc5f537ee9c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.ConditionalAccess.Policies
    .Request()
    .Filter("displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'")
    .GetAsync();

```