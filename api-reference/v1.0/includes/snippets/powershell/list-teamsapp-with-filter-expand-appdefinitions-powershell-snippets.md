---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce31b0f9ed7e343e75841a0014a07238cb41fd6e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101944"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgAppCatalogTeamApp -Filter "id eq '876df28f-2e78-423b-94a5-44181bd0e225'" -ExpandProperty "appDefinitions" 

```