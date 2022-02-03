---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 08104e6d70a790cecbb39444a33d5fb900c341c1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349403"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Remove-MgUserOnlineMeetingRegistrationCustomQuestion -UserId $userId -OnlineMeetingId $onlineMeetingId -MeetingRegistrationQuestionId $meetingRegistrationQuestionId

```