---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a3349af58adefbfc9cb40803197b301dd6b3ecd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = await graphClient.Print.Connectors["{printConnector-id}"]
    .Request()
    .GetAsync();

```