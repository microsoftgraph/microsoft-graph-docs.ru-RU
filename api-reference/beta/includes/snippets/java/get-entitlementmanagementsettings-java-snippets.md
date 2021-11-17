---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1639eb0212f9dfc08cf4190e4f8438ba52045ef4a5b65e0229bc9eb53069462
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256283"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EntitlementManagementSettings entitlementManagementSettings = graphClient.identityGovernance().entitlementManagement().settings()
    .buildRequest()
    .get();

```