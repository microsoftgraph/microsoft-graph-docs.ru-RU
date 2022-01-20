---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ff4e2a38ceaa0500de976611682b36cded68cdb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114777"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Description = "Library Assist"
    DisplayName = "Library Assist"
    GroupTypes = @(
        "Unified"
    )
    MailEnabled = $true
    MailNickname = "library-help"
}

Update-MgGroup -GroupId $groupId -BodyParameter $params

```