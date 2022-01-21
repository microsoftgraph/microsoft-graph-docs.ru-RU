---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d7437517dbd4e4ea6a02dfba922ff71ecf0d7ca
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090315"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Remove-MgComplianceEdiscoveryCaseTag -CaseId $caseId -TagId $tagId -Forcedelete true 

```