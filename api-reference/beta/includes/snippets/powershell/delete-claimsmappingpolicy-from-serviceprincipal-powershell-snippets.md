---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2643e23eae93f7633ce4c5ee9112ae4aea9321fe
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445384"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgServicePrincipalClaimMappingPolicyByRef -ServicePrincipalId $servicePrincipalId -ClaimsMappingPolicyId $claimsMappingPolicyId

```