---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cfb2e25b8f08dcb910cfbd49a4bf5b64953cc917
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945295"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequests = await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests
    .Request()
    .GetAsync();

```