---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79aa126ae974b60b7f4490ff6aedb90eb4618b00b3b29ccef60878c8bed5a6c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57315526"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionPage members = graphClient.chats("{id}").members()
    .buildRequest()
    .get();

```