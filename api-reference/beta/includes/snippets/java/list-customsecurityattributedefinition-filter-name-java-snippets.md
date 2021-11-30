---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b9539b4c09861e68631094b891f21d366eedc91
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224650"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinitionCollectionPage customSecurityAttributeDefinitions = graphClient.directory().customSecurityAttributeDefinitions()
    .buildRequest()
    .filter("name eq 'Project' and status eq 'Available'")
    .get();

```