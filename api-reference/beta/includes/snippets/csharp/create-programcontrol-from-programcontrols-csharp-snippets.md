---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d9ad6727ad4bb483bf9937cc660225521efd67d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControl = new ProgramControl
{
    ControlId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    ControlTypeId = "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    ProgramId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
};

await graphClient.ProgramControls
    .Request()
    .AddAsync(programControl);

```