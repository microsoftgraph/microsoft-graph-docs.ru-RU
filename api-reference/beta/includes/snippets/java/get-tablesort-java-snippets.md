---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8a9a9ab1f3b3aafd6b7482902670b13c8387a9d3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967334"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableSort workbookTableSort = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .buildRequest()
    .get();

```