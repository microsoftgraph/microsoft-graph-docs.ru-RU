---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc5fc52868bb953a6b997223846c4ee6f9643e78
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094692"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = await graphClient.Sites["{site-id}"].TermStore
    .Request()
    .GetAsync();

```