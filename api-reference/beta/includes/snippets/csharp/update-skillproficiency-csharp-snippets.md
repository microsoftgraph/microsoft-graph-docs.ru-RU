---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 608410a75e85dded6d073d79536c8d04bf3f55c3
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = new SkillProficiency
{
    Categories = new List<String>()
    {
        "categories-value"
    },
    DisplayName = "displayName-value",
    Proficiency = SkillProficiencyLevel.Elementary,
    WebUrl = "webUrl-value"
};

await graphClient.Me.Profile.Skills["{id}"]
    .Request()
    .UpdateAsync(skillProficiency);

```