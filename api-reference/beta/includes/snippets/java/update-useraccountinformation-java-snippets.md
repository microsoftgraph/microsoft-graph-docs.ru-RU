---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 000fa1008efe9091edbf5b501426ca819d3ae81a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967148"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformation userAccountInformation = new UserAccountInformation();
userAccountInformation.countryCode = "NO";

graphClient.me().profile().account("{id}")
    .buildRequest()
    .patch(userAccountInformation);

```