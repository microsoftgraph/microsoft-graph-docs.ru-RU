---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 894ef9959820637dc4484b7fc7bc89ac16f0297d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093970"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    IssuingAuthority = "International Academy of Marketing Excellence"
    IssuingCompany = "International Academy of Marketing Excellence"
}

Update-MgUserProfileCertification -UserId $userId -PersonCertificationId $personCertificationId -BodyParameter $params

```