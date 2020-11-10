---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c3e8835d2a77439edd8f3374d85717d52cedc42
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959465"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

RecordingStatus status = RecordingStatus.NOT_RECORDING;

graphClient.communications().calls("{id}")
    .updateRecordingStatus(status,clientContext)
    .buildRequest()
    .post();

```