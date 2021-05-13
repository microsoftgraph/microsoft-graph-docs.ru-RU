---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 436e5953610661cd17acec61b6cb810d4af7f795
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474024"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().entitlementManagement().accessPackageAssignments()
    .filterByCurrentUser(AccessPackageAssignmentFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('target')
        .build())
    .buildRequest()
    .get();

```