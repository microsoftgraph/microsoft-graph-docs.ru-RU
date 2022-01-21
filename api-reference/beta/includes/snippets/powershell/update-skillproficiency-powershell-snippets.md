---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cd628f39dc0b14c632f459d591887583581c0d2c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125249"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Professional"
    )
    Proficiency = "advancedProfessional"
}

Update-MgUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId -BodyParameter $params

```