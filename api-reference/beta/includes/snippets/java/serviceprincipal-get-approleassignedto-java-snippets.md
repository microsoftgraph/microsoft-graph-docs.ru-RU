---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5404a1cf230138bbfdc869400aeea3cd877b44f160bac700d8ffa86f90918598
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139670"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignedTo = graphClient.servicePrincipals("8e881353-1735-45af-af21-ee1344582a4d").appRoleAssignedTo()
    .buildRequest()
    .get();

```