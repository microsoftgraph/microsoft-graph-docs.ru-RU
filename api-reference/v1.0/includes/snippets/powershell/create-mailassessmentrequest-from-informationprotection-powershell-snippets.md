---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2942b77785bf48af10d03a2809506a288b070f2b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134718"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.mailAssessmentRequest"
    RecipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com"
    ExpectedAssessment = "block"
    Category = "spam"
    MessageUri = "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```