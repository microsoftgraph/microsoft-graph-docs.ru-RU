---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f14661e3975617002361abc2007e7116d9944f9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCompatibleHubContentTypes = await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .GetCompatibleHubContentTypes()
    .Request()
    .GetAsync();

```