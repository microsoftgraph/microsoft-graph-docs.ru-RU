---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31f67d785b93ca1b26f3f50e77daaeedd745c6b5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117661"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Fabrikam Arts High School"
    Description = "Magnate school for the arts. Los Angeles School District"
}

Update-MgEducationSchool -EducationSchoolId $educationSchoolId -BodyParameter $params

```