---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d970bc9795870f614e2be4a3f66400c3ced62cc4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125200"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationSoftwareOathMethod -UserId $userId -SoftwareOathAuthenticationMethodId $softwareOathAuthenticationMethodId

```