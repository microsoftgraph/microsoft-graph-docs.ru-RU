---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5bacebebd2a2b476b7cb1fe90103fb2496f55c4e957472f262aeed0bf72e281e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57317470"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NotebookCollectionPage notebooks = graphClient.me().onenote().notebooks()
    .buildRequest()
    .get();

```