---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5bf89a8cceaaa19531e9ca0572e77aa24b10e8c3e92738dcbaf61fa9ad15d225
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57153174"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String shift = "shift-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .insert(WorkbookRangeInsertParameterSet
        .newBuilder()
        .withShift(shift)
        .build())
    .buildRequest()
    .post();

```