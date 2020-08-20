---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2186fe6f8c0c931c458930edafaf99e5c288f673
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821403"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = new SkillProficiency
{
    Categories = new List<String>()
    {
        "Professional"
    },
    Proficiency = SkillProficiencyLevel.AdvancedProfessional
};

await graphClient.Me.Profile.Skills["{id}"]
    .Request()
    .UpdateAsync(skillProficiency);

```