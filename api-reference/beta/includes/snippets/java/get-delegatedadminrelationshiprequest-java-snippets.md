---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ba326d00683079e69c8184600ddd9bdb4aafa7a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209177"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminRelationshipRequest delegatedAdminRelationshipRequest = graphClient.tenantRelationships().delegatedAdminRelationships("5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836").requests("cf4a23c7-070c-4d1c-8be8-1e86085ac9d1")
    .buildRequest()
    .get();

```