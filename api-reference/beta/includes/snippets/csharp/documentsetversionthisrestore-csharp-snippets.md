---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5636a379b642fa8f7826d77ca763b12db6700131
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].DocumentSetVersions["{documentSetVersion-id}"]
    .Restore()
    .Request()
    .PostAsync();

```