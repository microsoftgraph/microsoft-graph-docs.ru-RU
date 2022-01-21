---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6bbcfe7a5d24b2e9fcf81c025999f50e1990733c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107486"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    IsRead = $true
}

Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```