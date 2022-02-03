---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 73f58fb9dbf9a87d7e6aa2bafdae9aa7cf454052
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339278"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "clientContext-value"
}

Stop-MgCommunicationCallMediaProcessing -CallId $callId -BodyParameter $params

```