---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 28fcccc67c51d5e4b23de2d85b2380c8a7d27d793aee0ae6c38c5975545ae6e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmission = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Request()
    .GetAsync();

```