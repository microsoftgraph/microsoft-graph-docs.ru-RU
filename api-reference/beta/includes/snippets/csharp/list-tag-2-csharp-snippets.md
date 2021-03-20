---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a53e4236eb157bc178e66614a4a3512dad2d713e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952009"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childTags = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags["{ediscovery.tag-id}"].ChildTags
    .Request()
    .GetAsync();

```