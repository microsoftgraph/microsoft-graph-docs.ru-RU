---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d1ba644236257b4604ad729cf311b28a1fc1b797
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112893"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "extensions(`$filter=id eq 'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')" 

```