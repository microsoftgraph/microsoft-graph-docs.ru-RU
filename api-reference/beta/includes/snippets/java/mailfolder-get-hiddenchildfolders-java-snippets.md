---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2507e9e91db12a76b803653fa2d74bdb82ba98af1f9eb1e3914094ee4dacd1c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252839"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("includeHiddenFolders", "true"));

MailFolderCollectionPage childFolders = graphClient.me().mailFolders("AAMkAGVmMDEzM").childFolders()
    .buildRequest( requestOptions )
    .get();

```