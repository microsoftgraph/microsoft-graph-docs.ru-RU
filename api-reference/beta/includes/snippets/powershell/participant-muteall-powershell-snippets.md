---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 022827babdf170f36f54e2bbaf6d1f330d6f96f2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502542"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Participants = @(
        ""
    )
    ClientContext = "clientContext-value"
}

Invoke-MgMuteAllCommunicationCallParticipant -CallId $callId -BodyParameter $params

```