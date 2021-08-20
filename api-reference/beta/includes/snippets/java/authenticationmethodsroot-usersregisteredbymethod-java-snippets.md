---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8fcd3edf406a698391ef3b65885451837da44740e37eb58ab55888857cbdb0e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserRegistrationMethodSummary userRegistrationMethodSummary = graphClient.reports().authenticationMethods()
    .usersRegisteredByMethod(AuthenticationMethodsRootUsersRegisteredByMethodParameterSet
        .newBuilder()
        .withIncludedUserTypes('all')
        .withIncludedUserRoles('all')
        .build())
    .buildRequest()
    .get();

```