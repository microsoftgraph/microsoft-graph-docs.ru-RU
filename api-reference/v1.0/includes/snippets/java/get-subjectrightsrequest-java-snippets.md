---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8f63c6ee6be8babd489b7ba2ed4ca345f457b33d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687660"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubjectRightsRequest subjectRightsRequest = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .buildRequest()
    .get();

```