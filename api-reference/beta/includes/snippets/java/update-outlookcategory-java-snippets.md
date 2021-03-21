---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: da93dbc4b9b2282e11cc86af55395dfba64baa34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = new OutlookCategory();
outlookCategory.color = CategoryColor.PRESET15;

graphClient.me().outlook().masterCategories("bac262b7-485d-4739-b436-e31467d64fac")
    .buildRequest()
    .patch(outlookCategory);

```