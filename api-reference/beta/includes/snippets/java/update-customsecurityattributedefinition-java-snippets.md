---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eaeca549952a8e48620dd6ebb51038dd3cfc5926
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225650"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinition customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition();
customSecurityAttributeDefinition.description = "Target completion date (YYYY/MM/DD)";

graphClient.directory().customSecurityAttributeDefinitions("Engineering_ProjectDate")
    .buildRequest()
    .patch(customSecurityAttributeDefinition);

```