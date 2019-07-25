---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7fd44ff55634340b2b0d9ede03fd05f4d6d67d62
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892776"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISectionGroupCollectionPage sectionGroups = graphClient.me().onenote().notebooks("{id}").sectionGroups()
    .buildRequest()
    .get();

```