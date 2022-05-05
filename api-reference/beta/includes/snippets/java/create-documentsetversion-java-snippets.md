---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d7fc5cc96484880eaa1b8818c5742b2155899ad
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211507"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DocumentSetVersion documentSetVersion = new DocumentSetVersion();
documentSetVersion.comment = "v1";
documentSetVersion.shouldCaptureMinorVersion = false;

graphClient.sites("root").lists("Documents").items("2").documentSetVersions()
    .buildRequest()
    .post(documentSetVersion);

```