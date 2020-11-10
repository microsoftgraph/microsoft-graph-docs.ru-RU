---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5f4fa45570dfe20e829e35a4ce15214f4a6b269c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980636"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignedTo = graphClient.servicePrincipals("{id}").appRoleAssignedTo()
    .buildRequest()
    .get();

```