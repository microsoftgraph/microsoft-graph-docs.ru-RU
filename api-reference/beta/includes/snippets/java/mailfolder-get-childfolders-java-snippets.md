---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff1d2cea03087895d5c7fcc90fd51c56732bd847
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981089"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolderCollectionPage childFolders = graphClient.me().mailFolders("AAMkAGVmMDEzM").childFolders()
    .buildRequest()
    .get();

```