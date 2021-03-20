---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 37009a0b1fb762dc139b5337159a619a2469133c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969470"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationFeedbackOutcome educationOutcome = new EducationFeedbackOutcome();
EducationFeedback feedback = new EducationFeedback();
EducationItemBody text = new EducationItemBody();
text.content = "This is feedback for the assignment as a whole.";
text.contentType = BodyType.TEXT;
feedback.text = text;
educationOutcome.feedback = feedback;

graphClient.education().me().assignments("{id}").submissions("{id}").outcomes("{id}")
    .buildRequest()
    .patch(educationOutcome);

```