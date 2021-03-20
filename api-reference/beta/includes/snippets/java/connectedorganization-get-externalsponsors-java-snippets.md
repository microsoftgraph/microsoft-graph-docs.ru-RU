---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7fb5de73e4fb8907d8834dba623296f7de6e7f44
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971685"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionPage externalSponsors = graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").externalSponsors()
    .buildRequest()
    .get();

```