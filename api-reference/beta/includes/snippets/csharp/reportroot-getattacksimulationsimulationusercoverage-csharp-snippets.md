---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4b040684ea66f3d75487800908dbdfa10dbdeb13
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996387"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAttackSimulationSimulationUserCoverage = await graphClient.Reports
    .GetAttackSimulationSimulationUserCoverage()
    .Request()
    .GetAsync();

```