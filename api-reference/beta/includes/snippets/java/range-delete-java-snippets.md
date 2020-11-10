---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5c2b940d5535729987d1a255a38ef784f6f4a9e9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974545"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String shift = "shift-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .delete(shift)
    .buildRequest()
    .post();

```