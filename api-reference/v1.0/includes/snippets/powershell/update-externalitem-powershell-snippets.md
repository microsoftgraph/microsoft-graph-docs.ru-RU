---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ab2f359e97ee32edc571298cba4c913fbda172fc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439315"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Acl = @(
        @{
            Type = "everyone"
            Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d"
            AccessType = "grant"
        }
    )
}

Update-MgExternalConnectionItem -ExternalConnectionId $externalConnectionId -ExternalItemId $externalItemId -BodyParameter $params

```