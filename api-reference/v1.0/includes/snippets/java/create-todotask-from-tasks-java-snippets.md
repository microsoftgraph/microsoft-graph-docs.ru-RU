---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1aab73d7371788ab3b7c0a7c8cb4ac6d113d7fa7
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65947029"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTask todoTask = new TodoTask();
todoTask.title = "A new task";
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Important");
todoTask.categories = categoriesList;
LinkedList<LinkedResource> linkedResourcesList = new LinkedList<LinkedResource>();
LinkedResource linkedResources = new LinkedResource();
linkedResources.webUrl = "http://microsoft.com";
linkedResources.applicationName = "Microsoft";
linkedResources.displayName = "Microsoft";
linkedResourcesList.add(linkedResources);
LinkedResourceCollectionResponse linkedResourceCollectionResponse = new LinkedResourceCollectionResponse();
linkedResourceCollectionResponse.value = linkedResourcesList;
LinkedResourceCollectionPage linkedResourceCollectionPage = new LinkedResourceCollectionPage(linkedResourceCollectionResponse, null);
todoTask.linkedResources = linkedResourceCollectionPage;

graphClient.me().todo().lists("AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM").tasks()
    .buildRequest()
    .post(todoTask);

```