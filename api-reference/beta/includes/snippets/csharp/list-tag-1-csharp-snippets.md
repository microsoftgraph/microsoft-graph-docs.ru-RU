---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e16307e33185fd2bacca0b25bc35949ba7a65cb7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946392"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tags = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags
    .Request()
    .GetAsync();

```