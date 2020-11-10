---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3effef6b85d931b8279a7be44ee0f909004716de
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951653"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewCollectionPage accessReviews = graphClient.accessReviews()
    .buildRequest()
    .filter("businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68',")
    .skip(0)
    .top(100)
    .get();

```