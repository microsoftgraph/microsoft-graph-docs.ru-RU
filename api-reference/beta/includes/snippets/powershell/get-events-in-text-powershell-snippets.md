---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ed2e554ffd7d91f5a11b7473fb889d9c8a4a2188
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130576"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEvent -UserId $userId -Property "subject,body,bodyPreview" 

```