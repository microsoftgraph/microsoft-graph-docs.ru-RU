---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b0a3379a132e5d758b941aaf7612bcc1aae6e08f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094562"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    "@odata.type" = "#microsoft.graph.bookingCustomQuestion"
    DisplayName = "What is your age?"
    AnswerInputType = "text"
    AnswerOptions = @(
    )
}

Update-MgBookingBusinessCustomQuestion -BookingBusinessId $bookingBusinessId -BookingCustomQuestionId $bookingCustomQuestionId -BodyParameter $params

```