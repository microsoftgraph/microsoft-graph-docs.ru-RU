---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a4a6ecf8cc024f49fb0e19d4d0681e68d4f7bf7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106038"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupTransitiveMemberOf -GroupId $groupId

```