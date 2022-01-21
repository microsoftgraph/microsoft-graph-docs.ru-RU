---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1587cedae56b34a0d74c0514241d0c6b17fdfbf0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122182"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Rogelio Cazares"
    GivenName = "Rogelio"
    MiddleName = "Fernando"
    Surname = "Cazares"
}

Update-MgEducationUser -EducationUserId $educationUserId -BodyParameter $params

```