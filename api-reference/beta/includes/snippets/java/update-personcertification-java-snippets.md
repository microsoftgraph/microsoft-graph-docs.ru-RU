---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c1f93f56d46714c520a53d7cc494d4dc32bb7358
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774602"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCertification personCertification = new PersonCertification();
personCertification.issuingAuthority = "International Academy of Marketing Excellence";
personCertification.issuingCompany = "International Academy of Marketing Excellence";

graphClient.users("{userId}").profile().certifications("{id}")
    .buildRequest()
    .patch(personCertification);

```