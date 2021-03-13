---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a3349af58adefbfc9cb40803197b301dd6b3ecd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = await graphClient.Print.Connectors["{printConnector-id}"]
    .Request()
    .GetAsync();

```