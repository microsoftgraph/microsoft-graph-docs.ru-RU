---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 552904a533e590df1326eeaefe89185583030626
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208972"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SwapShiftsChangeRequest swapShiftsChangeRequest = graphClient.teams("{teamId}").schedule().swapShiftsChangeRequests("{swapShiftsChangeRequestId}")
    .buildRequest()
    .get();

```