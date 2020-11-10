---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b08e6b5df90e0afb938a469ab52514291fdb5c99
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978654"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookTableRowCollectionPage rows = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows()
    .buildRequest()
    .get();

```