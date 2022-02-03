---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff33b38a61a71addef5a9a382ab00c207c56e89d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340331"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Reason = "none"
}

Invoke-MgRejectCommunicationCall -CallId $callId -BodyParameter $params

```