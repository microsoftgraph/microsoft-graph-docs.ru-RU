---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 84e37065c4f8321c8307e00bce2b64d42ff5a808
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099909"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        DisplayName = "Wikipedia"
        Link = "https://en.wikipedia.org/wiki/Main_Page"
        "@odata.type" = "#microsoft.graph.educationLinkResource"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```