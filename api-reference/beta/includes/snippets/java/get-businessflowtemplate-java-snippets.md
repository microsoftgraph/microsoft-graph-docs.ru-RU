---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 084d492264a5847b397de4cfdb17066d203f3e39713ca25f4e59c82ed8067110
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57142575"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BusinessFlowTemplateCollectionPage businessFlowTemplates = graphClient.businessFlowTemplates()
    .buildRequest()
    .get();

```