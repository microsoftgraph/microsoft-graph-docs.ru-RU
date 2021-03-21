---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6995aee40865b46beff7231ff994d007bf38413e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978986"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = new PrivilegedApproval();
privilegedApproval.approvalState = ApprovalState.PENDING;
privilegedApproval.approverReason = "approverReason-value";

graphClient.privilegedApproval("{requestId}")
    .buildRequest()
    .patch(privilegedApproval);

```