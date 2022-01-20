---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 102768facb2e2db4888015b5fd31574e958a56a7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126615"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyTokenLifetimePolicy -TokenLifetimePolicyId $tokenLifetimePolicyId

```