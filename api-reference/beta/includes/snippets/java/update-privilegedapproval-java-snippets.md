---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c3130fb2ad2ba9e9fe930d907f39ab6ab527906c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777652"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = new PrivilegedApproval();
privilegedApproval.approvalState = ApprovalState.PENDING;
privilegedApproval.approverReason = "approverReason-value";

graphClient.privilegedApproval("{requestId}")
    .buildRequest()
    .patch(privilegedApproval);

```