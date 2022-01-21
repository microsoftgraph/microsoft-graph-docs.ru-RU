---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 95633c37b048fdcbabc7da539a5101681eb3b367
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109267"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgIdentityConditionalAccessNamedLocation -Filter "microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')" 

```