---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: df79ffad8ca24d5f3eb77e5ea6a6cf57d1070895
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResource educationSubmissionResource = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("1618dfb0-3ff2-4edf-8d5c-b8f81df00e80").submissions("da443246-384d-673b-32db-bdba9d7f2b51").resources("c9169e8f-f096-4876-8675-7dee248af635")
    .buildRequest()
    .get();

```