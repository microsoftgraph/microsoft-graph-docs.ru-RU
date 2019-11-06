---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fb00cb7d3030cdec27be41698c5c7047cb36b2e7
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workPosition = await graphClient.Me.Profile.Positions["{id}"]
    .Request()
    .GetAsync();

```