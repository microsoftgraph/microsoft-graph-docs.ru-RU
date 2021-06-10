---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2b06a1ae35a47bc614c8d385b1d4f9072b2e4277
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinition unifiedRoleDefinition = graphClient.roleManagement().cloudPC().roleDefinitions("d40368cb-fbf4-4965-bbc1-f17b3a78e510")
    .buildRequest()
    .get();

```