---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: befc0ac6b5f8c1178b021788ffcd12cab3189c73
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = new LanguageProficiency
{
    AllowedAudiences = AllowedAudiences.Organization
};

await graphClient.Me.Profile.Languages["{id}"]
    .Request()
    .UpdateAsync(languageProficiency);

```