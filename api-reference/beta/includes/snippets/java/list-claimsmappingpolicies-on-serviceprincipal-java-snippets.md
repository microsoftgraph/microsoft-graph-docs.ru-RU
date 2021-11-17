---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7daf231ac4f5f876784fa00f2df4d16c2f2df44d6c7c1d0a0e89ad4318adbd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57247116"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicyCollectionWithReferencesPage claimsMappingPolicies = graphClient.servicePrincipals("{id}").claimsMappingPolicies()
    .buildRequest()
    .get();

```