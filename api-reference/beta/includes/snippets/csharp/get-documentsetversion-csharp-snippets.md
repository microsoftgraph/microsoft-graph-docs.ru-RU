---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fde54f95476da102e19293da4cc1282bba849bad
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var documentSetVersion = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].DocumentSetVersions["{documentSetVersion-id}"]
    .Request()
    .GetAsync();

```