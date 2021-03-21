---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 89b551d7c1aa9b40e46f5d1bee0ca4af135d811e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "id,name,lastModifiedDateTime"));
requestOptions.add(new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))"));

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest( requestOptions )
    .get();

```