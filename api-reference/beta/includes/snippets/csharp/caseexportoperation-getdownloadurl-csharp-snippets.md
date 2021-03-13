---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0c29cbc3591124ae904368b30bac0a530930c7d6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773265"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Operations["{ediscovery.caseOperation-id}"]
    .GetDownloadUrl()
    .Request()
    .GetAsync();

```