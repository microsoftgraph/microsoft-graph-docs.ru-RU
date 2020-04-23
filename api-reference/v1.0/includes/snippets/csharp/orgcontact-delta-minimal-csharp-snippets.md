---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e79da0abb76b07ab22b2da38b50124733300e1d
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.Mail 
             })
    .GetAsync();

```