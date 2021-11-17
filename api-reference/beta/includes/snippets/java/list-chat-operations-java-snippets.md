---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a54ee504fece591641acd05cd39308a5a72f15045f671e156a76b9043adb52c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57205139"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAsyncOperationCollectionPage operations = graphClient.chats("19:c253a29b5f694b55a6baad8e83510af7@thread.v2").operations()
    .buildRequest()
    .get();

```