---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 86dab50a1a38c724ac800266269632fd92d72dce73a5271392e864cc33a80872
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144564"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationOutcomeCollectionPage outcomes = graphClient.education().classes("{id}").assignments("{id}").submissions("{id}").outcomes()
    .buildRequest()
    .get();

```