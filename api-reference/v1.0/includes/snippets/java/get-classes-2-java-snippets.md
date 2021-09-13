---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6678d489d9517c2b47a3ba1004b27007e2a781ae00322278b27ae66e8aec426f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140392"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage classes = graphClient.education().schools("{school-id}").classes()
    .buildRequest()
    .get();

```