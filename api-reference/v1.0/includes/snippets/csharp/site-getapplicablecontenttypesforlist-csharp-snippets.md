---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2b8bd1fe3e29289dcacd66a5a0b45acbc4d27fd6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59085008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getApplicableContentTypesForList = await graphClient.Sites["{site-id}"]
    .GetApplicableContentTypesForList("listId")
    .Request()
    .GetAsync();

```