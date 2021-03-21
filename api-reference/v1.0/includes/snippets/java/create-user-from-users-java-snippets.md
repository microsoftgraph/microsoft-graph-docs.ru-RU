---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ea175c972208a4fceb89e790f3716112117d706
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972822"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.accountEnabled = true;
user.displayName = "Adele Vance";
user.mailNickname = "AdeleV";
user.userPrincipalName = "AdeleV@contoso.onmicrosoft.com";
PasswordProfile passwordProfile = new PasswordProfile();
passwordProfile.forceChangePasswordNextSignIn = true;
passwordProfile.password = "xWwvJ]6NMw+bWH-d";
user.passwordProfile = passwordProfile;

graphClient.users()
    .buildRequest()
    .post(user);

```