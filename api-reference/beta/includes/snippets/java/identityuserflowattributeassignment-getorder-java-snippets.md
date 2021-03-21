---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6579b18385bfc1a5ee19feb7892f879552dba93
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977300"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssignmentOrder assignmentOrder = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments()
    .getOrder()
    .buildRequest()
    .get();

```