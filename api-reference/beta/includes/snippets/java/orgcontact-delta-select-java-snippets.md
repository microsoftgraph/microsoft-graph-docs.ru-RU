---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c76b8e123b3887fe83400d57dfbeb8b808fc7aa461c5562b3129a7b54d19ebee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57212066"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContactDeltaCollectionPage delta = graphClient.contacts()
    .delta()
    .buildRequest()
    .select("displayName,jobTitle,mail")
    .get();

```