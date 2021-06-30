---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d8f05e7cd5692785007a3db86e82ed5f2ce19cc
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceHealth = await graphClient.Admin.ServiceAnnouncement.HealthOverviews["{serviceHealth-id}"]
    .Request()
    .Expand("issues")
    .GetAsync();

```