---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 493a97744d4af164b9308c3c5b7a6b6f621402519b946b356b8903fd2ace4fba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57373090"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = new PrintTaskTrigger();
printTaskTrigger.event = PrintEvent.JOB_STARTED;
printTaskTrigger.additionalDataManager().put("definition@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"));

graphClient.print().printers("{printerId}").taskTriggers()
    .buildRequest()
    .post(printTaskTrigger);

```