---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a8ab5c054f27c5980043202df7bf6dee6444e3e
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869963"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultiple unifiedRoleAssignmentMultiple = graphClient.roleManagement().cloudPC().roleAssignments("dbe9d288-fd87-41f4-b33d-b498ed207096")
    .buildRequest()
    .expand("roleDefinition")
    .get();

```