---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 82902ea1f13c8ba3d9a3b7becaf3ea5099c7a0f2c6853589d4fdb68674e5e772
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57248406"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "String";

graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .abort(PrintJobAbortParameterSet
        .newBuilder()
        .withReason(reason)
        .build())
    .buildRequest()
    .post();

```