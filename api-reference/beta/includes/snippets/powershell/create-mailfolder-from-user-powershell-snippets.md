---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 67bb4b348c4186184b16cb918c3aa09aed87dc0f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126600"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "Clutter"
    IsHidden = $true
}

New-MgUserMailFolder -UserId $userId -BodyParameter $params

```