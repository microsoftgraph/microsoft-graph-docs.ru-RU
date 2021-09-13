---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 57a84bf45fd307db68aa92b5b0a93649309c3ccf86b9d8490273b1e443c01d38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57197172"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SwapShiftsChangeRequest swapShiftsChangeRequest = graphClient.teams("{teamId}").schedule().swapShiftsChangeRequests("{swapShiftsChangeRequestId}")
    .buildRequest()
    .get();

```