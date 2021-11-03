---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c7fd0b39b8fc09e60c889ef1092d0995e03967c8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60718489"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContinuousAccessEvaluationPolicy continuousAccessEvaluationPolicy = new ContinuousAccessEvaluationPolicy();
continuousAccessEvaluationPolicy.migrate = true;

graphClient.identity().continuousAccessEvaluationPolicy()
    .buildRequest()
    .patch(continuousAccessEvaluationPolicy);

```