---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ad8f0a29109a831002f777b43f5bda594eaaa3da1b190905f83b9b6a1b456ca9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57192921"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("+1 425 555 0109");
user.businessPhones = businessPhonesList;
user.officeLocation = "18/2111";

graphClient.users("{id}")
    .buildRequest()
    .patch(user);

```