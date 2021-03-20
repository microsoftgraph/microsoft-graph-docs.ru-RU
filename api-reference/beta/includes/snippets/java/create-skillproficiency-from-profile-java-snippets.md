---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eb10c18fe88973e499bcc8b06ff64a9e29ff49fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977937"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SkillProficiency skillProficiency = new SkillProficiency();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Professional");
skillProficiency.categories = categoriesList;
skillProficiency.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);
skillProficiency.displayName = "API Design";
skillProficiency.proficiency = SkillProficiencyLevel.GENERAL_PROFESSIONAL;
LinkedList<String> collaborationTagsList = new LinkedList<String>();
collaborationTagsList.add("ableToMentor");
skillProficiency.collaborationTags = collaborationTagsList;

graphClient.me().profile().skills()
    .buildRequest()
    .post(skillProficiency);

```