---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0a81db96c1cdae0090411e37b8e1d46e9eb73fdb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961904"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

graphClient.groups("{id}")
    .evaluateDynamicMembership(memberId)
    .buildRequest()
    .post();

```