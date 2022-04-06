---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0c0760c344b47dd8b4c676282317ff0b019322ee
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acceptances = await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"].Acceptances
    .Request()
    .GetAsync();

```