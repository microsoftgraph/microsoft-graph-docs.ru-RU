---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a2de862450a6da69f47d13e307f36f82bff278ab66fcf39881301ea008ab37b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144755"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinitionCollectionPage roleDefinitions = graphClient.roleManagement().cloudPC().roleDefinitions()
    .buildRequest()
    .get();

```