---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 89c9c1060dcfc994aaf0bdd59a17dffb803fbdf1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781964"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Resources["{educationAssignmentResource-id}"]
    .Request()
    .GetAsync();

```