---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 76268c097c3437de48fcc6551cc8e770901414a1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200959"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.content = "Hello World";
chatMessage.body = body;

graphClient.teams("{id}").channels("{id}").messages()
    .buildRequest()
    .post(chatMessage);

```