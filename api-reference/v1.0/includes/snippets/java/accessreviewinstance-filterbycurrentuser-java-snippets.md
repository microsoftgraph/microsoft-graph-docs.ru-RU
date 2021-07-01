---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4389c68cba324cffe9359dbe7ec5f21389650f11
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209862"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances()
    .filterByCurrentUser(AccessReviewInstanceFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .get();

```