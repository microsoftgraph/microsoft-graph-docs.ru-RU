---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1545dbde8edee17ca59d9d3ee4dbc32fac064a2b445280e0bf607599db86faed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipationCollectionPage projects = graphClient.me().profile().projects()
    .buildRequest()
    .get();

```