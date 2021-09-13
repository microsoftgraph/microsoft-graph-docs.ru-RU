---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79470a20ca68eebc733d4905d8644e4db9b4e4e1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147600"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Request()
    .GetAsync();

```