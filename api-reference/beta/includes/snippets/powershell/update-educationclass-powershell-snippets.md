---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3fa849ec305a8957e5c6db2000160a5bfdf088e3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106261"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Description = "History - World History 1"
    DisplayName = "World History Level 1"
}

Update-MgEducationClass -EducationClassId $educationClassId -BodyParameter $params

```