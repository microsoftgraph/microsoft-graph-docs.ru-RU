---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 068315922d0f1fa45b4026d0d4a7b0f582c6d52c5aec2186ae761b643d253c0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138677"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String storageLocation = "storageLocation-value";

graphClient.users("{id}")
    .exportPersonalData(UserExportPersonalDataParameterSet
        .newBuilder()
        .withStorageLocation(storageLocation)
        .build())
    .buildRequest()
    .post();

```