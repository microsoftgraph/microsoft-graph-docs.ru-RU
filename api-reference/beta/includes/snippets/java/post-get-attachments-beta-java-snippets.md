---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9993d3edf281e6e1842cf9385d461d719985b7f1c6b03cdfb72a87200309772d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322507"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentCollectionPage attachments = graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJfolA==").posts("AAMkADJ-aHAAA=").attachments()
    .buildRequest()
    .get();

```