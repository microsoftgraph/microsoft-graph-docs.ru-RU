---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ae54e7b94bc0fde0d4e53aaf511cbff827025a1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129464"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgServicePrincipalDelegatedPermissionClassification -ServicePrincipalId $servicePrincipalId -DelegatedPermissionClassificationId $delegatedPermissionClassificationId

```