---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a304d750b42dd6cc7204ed716cb12eb03b1017ae1248bb08349ece1a8a54b476
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57396999"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment();
identityUserFlowAttributeAssignment.userInputType = IdentityUserFlowAttributeInputType.TEXT_BOX;

graphClient.identity().b2xUserFlows("{b2xIdentityUserFlowId}").userAttributeAssignments("{id}")
    .buildRequest()
    .patch(identityUserFlowAttributeAssignment);

```