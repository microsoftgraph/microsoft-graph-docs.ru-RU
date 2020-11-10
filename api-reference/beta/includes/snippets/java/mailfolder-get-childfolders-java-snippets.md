---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 718ed26e82894cc19b2d1f4b38dd8f1752dd1249
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979359"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderCollectionPage childFolders = graphClient.me().mailFolders("AAMkAGVmMDEzM").childFolders()
    .buildRequest()
    .get();

```