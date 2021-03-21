---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79d0bfd46a1551e611503d3890e12c1a2c41e1cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975862"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = new PrintTask();
PrintTaskStatus status = new PrintTaskStatus();
status.state = PrintTaskProcessingState.COMPLETED;
status.description = "completed";
printTask.status = status;

graphClient.print().taskDefinitions("3203656e-6069-4e10-8147-d25290b00a3c").tasks("d036638b-1272-4bba-9227-732463823ed3")
    .buildRequest()
    .patch(printTask);

```