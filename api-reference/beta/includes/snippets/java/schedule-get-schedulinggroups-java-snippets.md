---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d4c0ec99fe2468aa72212a88caade7a56296d0bb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975765"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchedulingGroup schedulingGroup = graphClient.teams("{teamId}").schedule().schedulingGroups("{schedulingGroupId}")
    .buildRequest()
    .get();

```