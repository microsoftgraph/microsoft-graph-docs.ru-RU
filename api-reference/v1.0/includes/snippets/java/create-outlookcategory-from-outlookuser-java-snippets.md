---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d3d60e60cb51ae920c24e9beba9f1bf03c5f42b598c22f48eca69c24ee5c46d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57307485"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = new OutlookCategory();
outlookCategory.displayName = "Project expenses";
outlookCategory.color = CategoryColor.PRESET9;

graphClient.me().outlook().masterCategories()
    .buildRequest()
    .post(outlookCategory);

```