---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b1f72e2997fe37e1bc4d8ab08aafd98fc45e64d754a10b5886d249976e2b756e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140511"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserSettingCollectionPage userSettings = graphClient.deviceManagement().virtualEndpoint().userSettings()
    .buildRequest()
    .get();

```