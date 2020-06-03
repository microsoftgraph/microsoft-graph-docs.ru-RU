---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fa020232bafc4ce4471d5ccdef4df5bd4cffbc6f
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217429"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISwapShiftsChangeRequestCollectionPage swapShiftsChangeRequests = graphClient.teams("{teamId}").schedule().swapShiftsChangeRequests()
    .buildRequest()
    .get();

```