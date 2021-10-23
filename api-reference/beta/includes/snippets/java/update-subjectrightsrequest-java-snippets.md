---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 919287056f2de02c3fe4ee32b0111dced5c9f505
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559626"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubjectRightsRequest subjectRightsRequest = new SubjectRightsRequest();
subjectRightsRequest.internalDueDateTime = OffsetDateTimeSerializer.deserialize("2021-08-30T00:00:00Z");

graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .buildRequest()
    .patch(subjectRightsRequest);

```