---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 85c26e03ac305d01a2ea80cbb4a59d7aa3f00ea2
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610988"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelGetAllMessagesCollectionPage getAllMessages = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels()
    .getAllMessages()
    .buildRequest()
    .get();

```