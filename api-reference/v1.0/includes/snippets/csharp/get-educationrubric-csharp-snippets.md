---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bdff88ae21fc4db8ce489444cb53cb9ba5bbfe6006c815daca11795b15889412
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57317803"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .GetAsync();

```