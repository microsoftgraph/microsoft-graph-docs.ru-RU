---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cab9582fdc33a58dee1b4f0f3469609ab73676a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805833"
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

await graphClient.Me.Profile.Skills["{skillProficiency-id}"]
    .Request()
    .UpdateAsync(skillProficiency);

```