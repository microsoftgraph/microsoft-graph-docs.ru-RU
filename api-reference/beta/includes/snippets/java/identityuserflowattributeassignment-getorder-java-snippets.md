---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a56ee591f829d7474e77afbdf37cc779dfe643a2
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689263"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssignmentOrder assignmentOrder = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments()
    .getOrder()
    .buildRequest()
    .get();

```