---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2695042044d6f6fa273dfe271436b0fd8446b1302d44511288dfea0e4555890
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57432226"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchedulingGroup schedulingGroup = graphClient.teams("{teamId}").schedule().schedulingGroups("{schedulingGroupId}")
    .buildRequest()
    .get();

```