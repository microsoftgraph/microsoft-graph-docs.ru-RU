---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 050faef77a248943ae9c9ae8e9ef1d306b9e5eac
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473035"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmission = await graphClient.Education.Classes["11010"].Assignments["19002"].Submissions["33223"]
    .Request()
    .GetAsync();

```