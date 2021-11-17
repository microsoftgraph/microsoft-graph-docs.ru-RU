---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d24faea6ba552382f10ddc6286f73eb8ac9aa00e11a647534b52f1fc1e79857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138592"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequestCollectionPage accessPackageAssignmentRequests = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests()
    .buildRequest()
    .filter("(requestState eq 'PendingApproval')")
    .expand("requestor($expand=connectedOrganization)")
    .get();

```