---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 83a51d9c0e67373f529d6f59325c5e311f34b610
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130470"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignmentSubmission -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -ExpandProperty "*" 

```