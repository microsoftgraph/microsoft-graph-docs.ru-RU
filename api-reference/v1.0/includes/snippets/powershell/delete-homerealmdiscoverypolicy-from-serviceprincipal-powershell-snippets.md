---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3116564abda9eb838737f00f62bfca5b497f08a2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438489"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgServicePrincipalHomeRealmDiscoveryPolicyByRef -ServicePrincipalId $servicePrincipalId -HomeRealmDiscoveryPolicyId $homeRealmDiscoveryPolicyId

```