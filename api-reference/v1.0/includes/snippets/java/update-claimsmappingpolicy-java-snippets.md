---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ecdcad38f4681141d6e3150fe1fec0a00dfd195bdcbe6113369e437eb72171f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57319590"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
claimsMappingPolicy.definition = definitionList;
claimsMappingPolicy.displayName = "displayName-value";
claimsMappingPolicy.isOrganizationDefault = true;

graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .patch(claimsMappingPolicy);

```