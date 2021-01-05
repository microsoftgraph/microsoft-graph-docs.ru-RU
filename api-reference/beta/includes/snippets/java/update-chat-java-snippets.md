---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a7941bc7e08513726f59bc413ffda8d3814acc98
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753943"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = new Chat();
chat.topic = "Group chat title update";

graphClient.chats("19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2")
    .buildRequest()
    .patch(chat);

```