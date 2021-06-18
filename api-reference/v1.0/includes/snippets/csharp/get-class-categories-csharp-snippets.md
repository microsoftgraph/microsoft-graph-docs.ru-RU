---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b539b0d2ac478ea84e8c7d8ba2c5ed9391c6c61c
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993068"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentCategories = await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories
    .Request()
    .GetAsync();

```