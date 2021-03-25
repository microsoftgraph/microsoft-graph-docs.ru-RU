---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a85fca0f5a30c9cf77ede5b82d72f520f569643
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201501"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdminConsentRequestPolicy adminConsentRequestPolicy = graphClient.policies().adminConsentRequestPolicy()
    .buildRequest()
    .get();

```