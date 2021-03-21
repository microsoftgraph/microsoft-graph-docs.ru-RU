---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0da1d653d75a1c297488d1102ab82b000b16d9c2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OfferShiftRequest offerShiftRequest = graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .buildRequest()
    .get();

```