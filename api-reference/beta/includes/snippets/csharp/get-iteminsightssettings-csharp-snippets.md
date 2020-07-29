---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d7817bfcdc78de0b7f6aa98018cc16c2713508c
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509643"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemInsights = await graphClient.Organization["{organizationId}"].Settings.ItemInsights
    .Request()
    .GetAsync();

```