---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68c36b09fd8a807c27e51c5f4a518f4af3defb1b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776090"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShiftChangeRequest openShiftChangeRequest = graphClient.teams("{id}").schedule().openShiftChangeRequests("SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09")
    .buildRequest()
    .get();

```