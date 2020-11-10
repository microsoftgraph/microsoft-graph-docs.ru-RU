---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 472c8faaed6dbdc199d3d3498704539ba0656cba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963619"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
ItemReference parentReference = new ItemReference();
parentReference.id = "new-parent-folder-id";
driveItem.parentReference = parentReference;
driveItem.name = "new-item-name.txt";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```