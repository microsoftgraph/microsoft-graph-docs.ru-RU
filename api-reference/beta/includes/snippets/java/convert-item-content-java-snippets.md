---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d5155c57fb7fdb49a45c0542d02ee91028d5c80a9942829496cc39f588ddd94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364942"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("format", "{format}"));

InputStream stream = graphClient.customRequest("/drive/items/{item-id}/content", InputStream.class)
    .buildRequest( requestOptions )
    .get();

```