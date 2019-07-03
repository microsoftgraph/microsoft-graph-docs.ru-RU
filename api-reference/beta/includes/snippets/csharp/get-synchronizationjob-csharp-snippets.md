---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 382b5f7b10817364e410e9fa19e13e9ea2df588d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationJob = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Request()
    .GetAsync();

```