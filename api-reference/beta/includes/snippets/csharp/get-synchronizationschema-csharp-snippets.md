---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 029f568395f4db3997956bc93746c39ab5ba7ea2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = await graphClient.ServicePrincipals["{servicePrincipalId}"].Synchronization.Jobs["{jobId}"].Schema
    .Request()
    .Header("Authorization","Bearer {Token}")
    .GetAsync();

```