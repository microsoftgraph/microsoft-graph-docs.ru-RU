---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03966d3ead80ef4dc6a0be2ccc0dd10024860b5e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109814"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].TermStore.Groups["{termStore.group-id}"]
    .Request()
    .DeleteAsync();

```