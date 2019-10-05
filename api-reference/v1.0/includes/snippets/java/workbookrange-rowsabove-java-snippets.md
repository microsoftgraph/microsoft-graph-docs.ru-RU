---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3cfffc9082edeaaa2c9ace776bb03b8805b4004a
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402984"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(null)
    .buildRequest()
    .post();

```