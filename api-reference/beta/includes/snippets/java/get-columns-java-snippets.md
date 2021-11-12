---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f788b5a87099cc45b4d9914e1e8ff23ae9f97792dab80e80e4ed4291f9d05e62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57153154"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumnCollectionPage columns = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .buildRequest()
    .skip(5)
    .top(5)
    .get();

```