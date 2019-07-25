---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3debe5217c9da100fb7d53bbd05722f7ae47a227
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityRiskEvents = await graphClient.IdentityRiskEvents
    .Request()
    .GetAsync();

```