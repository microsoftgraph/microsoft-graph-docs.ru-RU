---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 70d76a6cd2b1ea8bb95c3114c8b2ce9f1a398b92
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179412"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewCollectionPage accessReviews = graphClient.accessReviews()
    .buildRequest()
    .filter("businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'")
    .skip(0)
    .top(100)
    .get();

```