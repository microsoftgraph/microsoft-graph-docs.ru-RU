---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b28814bc8df27abe7db3986f1bea7dda716b87a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208403"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

graphClient.groups("{id}")
    .evaluateDynamicMembership(GroupEvaluateDynamicMembershipParameterSet
        .newBuilder()
        .withMemberId(memberId)
        .build())
    .buildRequest()
    .post();

```