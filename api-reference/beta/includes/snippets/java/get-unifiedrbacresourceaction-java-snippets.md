---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c2fcec5897dfc743bff57f38f1de37aea54d7e73
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRbacResourceAction unifiedRbacResourceAction = graphClient.roleManagement().directory().resourceNamespaces("microsoft.directory").resourceActions("microsoft.directory-accessReviews-allProperties-read-get")
    .buildRequest()
    .get();

```