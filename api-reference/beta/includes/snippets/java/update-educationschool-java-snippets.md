---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 95fa3fc3dc072e0118bac9aa3a4cecfce20e8566
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955515"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = new EducationSchool();
educationSchool.displayName = "Fabrikam Arts High School";
educationSchool.description = "Magnate school for the arts. Los Angeles School District";

graphClient.education().schools("10002")
    .buildRequest()
    .patch(educationSchool);

```