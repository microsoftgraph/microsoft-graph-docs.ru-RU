---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f73deb5b3b3c44d48b91df863e90a4e19e7eb615
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.RiskDetections
    .Request()
    .GetAsync();

```