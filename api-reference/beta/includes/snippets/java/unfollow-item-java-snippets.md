---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 665a1a553b896793aab223324fca4edb72e36b05
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228370"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .unfollow()
    .buildRequest()
    .post();

```