---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9825e866780b3b362c4f8df28df16205e7a61a57
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610716"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ResourceSpecificPermissionGrantCollectionPage permissionGrants = graphClient.chats("19:089ac694c48647c68035aae675cf78ab@thread.v2").permissionGrants()
    .buildRequest()
    .get();

```