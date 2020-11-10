---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bad2b1fae7a93b8ec4507acfa3f4ae8d6652ff1b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967963"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = new OutlookCategory();
outlookCategory.displayName = "Project expenses";
outlookCategory.color = CategoryColor.PRESET9;

graphClient.me().outlook().masterCategories()
    .buildRequest()
    .post(outlookCategory);

```