---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 747c12b961ccd5e0e7639ec8c54e2f0666149876
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = new LanguageProficiency
{
    DisplayName = "Norwegian Bokmål",
    Tag = "nb-NO",
    Spoken = LanguageProficiencyLevel.NativeOrBilingual,
    Written = LanguageProficiencyLevel.NativeOrBilingual,
    Reading = LanguageProficiencyLevel.NativeOrBilingual
};

await graphClient.Me.Profile.Languages
    .Request()
    .AddAsync(languageProficiency);

```