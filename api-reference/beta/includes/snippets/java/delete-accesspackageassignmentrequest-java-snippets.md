---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0908d2dc9691fccd0320aaf7f11d7fc2e381660d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests("{id}")
    .buildRequest()
    .delete();

```