---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 037bf22d5515b41734e4beb8adda89bf674c0adf
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337953"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequest accessPackageAssignmentRequest = new AccessPackageAssignmentRequest();
accessPackageAssignmentRequest.requestType = AccessPackageRequestType.ADMIN_REMOVE;
AccessPackageAssignment assignment = new AccessPackageAssignment();
assignment.id = "a6bb6942-3ae1-4259-9908-0133aaee9377";
accessPackageAssignmentRequest.assignment = assignment;

graphClient.identityGovernance().entitlementManagement().assignmentRequests()
    .buildRequest()
    .post(accessPackageAssignmentRequest);

```