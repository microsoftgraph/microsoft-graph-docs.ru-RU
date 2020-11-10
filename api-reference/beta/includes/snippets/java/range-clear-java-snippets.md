---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68e747bf9da42fd85bad534b58ee60c91437c164
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978501"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String applyTo = "applyTo-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .clear(applyTo)
    .buildRequest()
    .post();

```