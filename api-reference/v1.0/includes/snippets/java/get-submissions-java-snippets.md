---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d222813b917a34fa5a5b7fbc06ca760ea99012ed
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767387"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionCollectionPage submissions = graphClient.education().classes("f4a941ff-9da6-4707-ba5b-0eae93cad0b4").assignments("3c77de7f-539b-49e1-9c96-1274f2f0ee3b").submissions()
    .buildRequest()
    .get();

```