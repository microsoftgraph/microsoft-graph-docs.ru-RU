---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88a90b2ec4f56212479c0b45179d424eb82e5b09
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339095"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRbacResourceActionCollectionPage resourceActions = graphClient.roleManagement().directory().resourceNamespaces("microsoft.directory").resourceActions()
    .buildRequest()
    .get();

```