---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03aa75e0e170dbeac75f499c5ed2d59f25ed7ad1675814190df199b1c2f6ccef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57309170"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .Filter("microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')")
    .GetAsync();

```