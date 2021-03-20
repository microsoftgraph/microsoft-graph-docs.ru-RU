---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 01e641f85f842cb1e0729f0fda4d9d83fc9b4fb3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969905"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = new EducationRubric();
educationRubric.displayName = "Example Credit Rubric after display name patch";

graphClient.education().me().rubrics("{id}")
    .buildRequest()
    .patch(educationRubric);

```