---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 600e4b95950f387d9ec5e194ad7ecea0d4c91a6d
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729957"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String password = "1234567890";

graphClient.users()
    .validatePassword(UserValidatePasswordParameterSet
        .newBuilder()
        .withPassword(password)
        .build())
    .buildRequest()
    .post();

```