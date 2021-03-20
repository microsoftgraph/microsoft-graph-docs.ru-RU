---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 71f4d2fcad1f1b393bb249eb49e4186e1929bb4e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972660"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.id = "123456!87";

graphClient.drive().bundles("{bundle-id}").children()
    .buildRequest()
    .post(driveItem);

```