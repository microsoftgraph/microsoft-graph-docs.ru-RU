---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5b7f034e1d119c08f6cf3f9a1bf61f8d7e38114f
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226022"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationUserAssignment -EducationUserId $educationUserId -ExpandProperty "submissions" 

```