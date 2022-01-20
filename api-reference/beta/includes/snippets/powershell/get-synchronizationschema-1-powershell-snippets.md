---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f3b4d512f1fb9c326ec983999f57f06ae3f1d69c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132711"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalSynchronizationJobSchema -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId

```