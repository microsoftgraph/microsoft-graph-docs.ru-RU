---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e9e579153b9182d57140111c00024ee32988e5926887948164a83d7dbe3da05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052314"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicy tokenLifetimePolicy = new TokenLifetimePolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
tokenLifetimePolicy.definition = definitionList;
tokenLifetimePolicy.displayName = "displayName-value";
tokenLifetimePolicy.isOrganizationDefault = true;

graphClient.policies().tokenLifetimePolicies()
    .buildRequest()
    .post(tokenLifetimePolicy);

```