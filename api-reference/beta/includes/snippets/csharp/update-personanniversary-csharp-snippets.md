---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 65ffb5614b5762f8e3508f1cd5a278784d519012
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnniversary = new PersonAnniversary
{
    AllowedAudiences = AllowedAudiences.Contacts
};

await graphClient.Me.Profile.Anniversaries["{id}"]
    .Request()
    .UpdateAsync(personAnniversary);

```