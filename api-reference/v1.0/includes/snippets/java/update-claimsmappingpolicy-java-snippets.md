---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a7c9429071f1e10c680bda4e4837a5b71e85165b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863219"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
claimsMappingPolicy.definition = definitionList;
claimsMappingPolicy.displayName = "displayName-value";
claimsMappingPolicy.isOrganizationDefault = true;
claimsMappingPolicy.type = "type-value";

graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .patch(claimsMappingPolicy);

```