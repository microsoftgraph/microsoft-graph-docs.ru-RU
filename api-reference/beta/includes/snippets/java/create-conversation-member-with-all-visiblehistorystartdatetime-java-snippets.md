---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a9bbc7c2f0d2bdf4836c02b1a27c26605edd2c2f216fca762f5900dcb375a554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144013"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"));
conversationMember.visibleHistoryStartDateTime = OffsetDateTimeSerializer.deserialize("0001-01-01T00:00:00Z");
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;

graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members()
    .buildRequest()
    .post(conversationMember);

```