---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e79936eb75dd3652656a7fc673d60565e4b0f25f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211093"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean _boolean = graphClient.teams("{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}").channels("19:33b76eea88574bd1969dca37e2b7a819@thread.skype")
    .doesUserHaveAccess(ChannelDoesUserHaveAccessParameterSet
        .newBuilder()
        .withUserPrincipalName("john.doe@contoso.com")
        .build())
    .buildRequest()
    .get();

```