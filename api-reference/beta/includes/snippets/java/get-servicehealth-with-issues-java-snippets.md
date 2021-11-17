---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 888f00ec6401f3b5e6994d5de0b67beddab411923778120bed3835d6c2ca95ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57314050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealth serviceHealth = graphClient.admin().serviceAnnouncement().healthOverviews("Microsoft 365 suite")
    .buildRequest()
    .expand("issues")
    .get();

```