---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f996d1d399db70f0fa216627c3ffe6ec96eab943
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776601"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollections = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections
    .Request()
    .GetAsync();

```