---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03406156ab6ca154b0b4ba86b1f1418ae987f49b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447341"
---
```powershell

Import-Module Microsoft.Graph.Reports

$params = @{
    RequestIds = @(
        "f01c6af6-6683-4a37-a945-0a925501eede"
        "42bf60ac-d0cb-4206-aa5c-101884298f55"
        "f09c8f14-8d8e-42cf-8a7e-732b0594e79b"
    )
}

Confirm-MgAuditLogSignInCompromised -BodyParameter $params

```