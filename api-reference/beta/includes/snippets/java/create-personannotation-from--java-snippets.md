---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f01d2b8d4c7978b65712fa11c9e2a878bf021127ea0c75edffb5ebc2e7556e7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57324520"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnotation personAnnotation = new PersonAnnotation();
ItemBody detail = new ItemBody();
detail.contentType = BodyType.TEXT;
detail.content = "I am originally from Australia, but grew up in Moscow, Russia.";
personAnnotation.detail = detail;
personAnnotation.displayName = "About Me";

graphClient.me().profile().notes()
    .buildRequest()
    .post(personAnnotation);

```