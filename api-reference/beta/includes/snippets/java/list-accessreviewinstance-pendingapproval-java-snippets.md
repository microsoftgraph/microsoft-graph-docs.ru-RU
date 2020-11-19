---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 30e51c526ada7c5b213bbb4ab74c42fc0f47aebc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222051"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewInstanceCollectionPage pendingAccessReviewInstances = graphClient.me().pendingAccessReviewInstances()
    .buildRequest()
    .expand("definition")
    .skip(0)
    .top(100)
    .get();

```