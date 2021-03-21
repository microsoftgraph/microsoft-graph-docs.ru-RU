---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1c0c905517b41558c8b9ea1494266f910b8a1a3b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema
    .Request()
    .Header("Authorization","Bearer {Token}")
    .GetAsync();

```