---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6f45ad00cd1f0c83d0f394687ead2a4718cc79f512691d6def30eef07c746ee3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252779"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OfferShiftRequest offerShiftRequest = graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .buildRequest()
    .get();

```