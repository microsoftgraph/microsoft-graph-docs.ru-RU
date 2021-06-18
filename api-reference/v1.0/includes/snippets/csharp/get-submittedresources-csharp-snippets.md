---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3433f20448b2014e96ed77f179499bbfe710ef94
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var submittedResources = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].SubmittedResources
    .Request()
    .GetAsync();

```