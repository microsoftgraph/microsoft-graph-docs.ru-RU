---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 004c30eb8d0e19cbacaf9be4422657f086122f0c667064d075bbb55d53fcfaf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57191340"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage incompatibleGroups = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleGroups()
    .buildRequest()
    .get();

```