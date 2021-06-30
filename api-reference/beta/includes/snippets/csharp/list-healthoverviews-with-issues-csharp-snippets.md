---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dca82b481e10afca0b4b6cf91e68487792c96069
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var healthOverviews = await graphClient.Admin.ServiceAnnouncement.HealthOverviews
    .Request()
    .Expand("issues")
    .GetAsync();

```