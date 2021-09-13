---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b93b8793812d76b644477eb3de61e4a92e37f7b42f95129ccf5d83251e9a5821
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152375"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookFormatProtection workbookFormatProtection = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().protection()
    .buildRequest()
    .get();

```