---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e328fd8b301ee7a96d1d6c6ef72c23f7d86229b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129282"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyTokenIssuancePolicy -TokenIssuancePolicyId $tokenIssuancePolicyId

```