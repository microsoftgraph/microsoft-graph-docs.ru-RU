---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc29cb5e95bc0e5a00180388bbb2547828a9cec2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970142"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedAccess("azureResources").roleAssignmentRequests("7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee")
    .updateRequest(GovernanceRoleAssignmentRequestUpdateRequestParameterSet
        .newBuilder()
        .withDecision(null)
        .withAssignmentState(null)
        .withSchedule(null)
        .withReason(null)
        .build())
    .buildRequest()
    .post();

```