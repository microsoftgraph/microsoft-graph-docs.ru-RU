---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b351fa2e29bed24e54d728640b16252f152299d2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228378"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "c300x400_crop"));

ThumbnailSetCollectionPage thumbnails = graphClient.me().drive().items("{item-id}").thumbnails()
    .buildRequest( requestOptions )
    .get();

```