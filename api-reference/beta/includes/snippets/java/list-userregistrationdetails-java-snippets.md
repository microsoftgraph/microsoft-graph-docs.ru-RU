---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4df8123966f1eb2d1d7d9ae5ebcd9c5fd1aedd7c
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224835"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserRegistrationDetailsCollectionPage userRegistrationDetails = graphClient.reports().authenticationMethods().userRegistrationDetails()
    .buildRequest()
    .get();

```