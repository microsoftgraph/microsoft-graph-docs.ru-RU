---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f2059e55c3c7a3337b4f75461506282f660728be
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991100"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var categories = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Categories
    .Request()
    .GetAsync();

```