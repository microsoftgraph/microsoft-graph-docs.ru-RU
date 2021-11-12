---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 250440bc6f7dc1f26d47a01b34efe39380e0eb7bb3c094af747ce3ec016ae491
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpointCollectionPage endpoints = graphClient.print().services("{id}").endpoints()
    .buildRequest()
    .get();

```