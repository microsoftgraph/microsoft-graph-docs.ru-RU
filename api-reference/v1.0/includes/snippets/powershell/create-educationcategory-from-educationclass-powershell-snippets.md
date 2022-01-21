---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 85a3c955e2f6adc5c1e87dd3b66475ff48ca27b8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136308"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Quizzes"
}

New-MgEducationClassAssignmentCategory -EducationClassId $educationClassId -BodyParameter $params

```