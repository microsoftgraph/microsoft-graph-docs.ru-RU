---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 53d3763acc3d5981c314affaa5d07bc5aa6ba483
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095004"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEventAttachment -UserId $userId -EventId $eventId -AttachmentId $attachmentId

```