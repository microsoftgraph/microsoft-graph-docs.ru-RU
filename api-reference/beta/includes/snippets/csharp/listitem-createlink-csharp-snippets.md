---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: efab48557e3f6e0d0c2f8eed759073cd70266682
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62138311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"]
    .CreateLink(type,null,null,null,null,null)
    .Request()
    .PostAsync();

```