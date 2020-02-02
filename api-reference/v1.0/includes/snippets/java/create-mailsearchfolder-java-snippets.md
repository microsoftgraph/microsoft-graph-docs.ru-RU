---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0552d7cedc6f04d17b02e5b60be492554750323e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544472"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailSearchFolder mailFolder = new MailSearchFolder();
mailFolder.displayName = "Weekly digests";
mailFolder.includeNestedFolders = true;
LinkedList<String> sourceFolderIdsList = new LinkedList<String>();
sourceFolderIdsList.add("AQMkADYAAAIBDAAAAA==");
mailFolder.sourceFolderIds = sourceFolderIdsList;
mailFolder.filterQuery = "contains(subject, 'weekly digest')";

graphClient.me().mailFolders("AQMkADYAAAIBDAAAAA==").childFolders()
    .buildRequest()
    .post(mailFolder);

```