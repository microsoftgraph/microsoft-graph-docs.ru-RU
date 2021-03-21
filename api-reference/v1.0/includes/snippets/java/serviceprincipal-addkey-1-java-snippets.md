---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d906bf433754a1b1ed7407248e7fe0475d33937e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959493"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

KeyCredential keyCredential = new KeyCredential();
keyCredential.type = "AsymmetricX509Cert";
keyCredential.usage = "Verify";
keyCredential.key = Base64.getDecoder().decode("MIIDYDCCAki...");



String proof = "eyJ0eXAiOiJ...";

graphClient.servicePrincipals("{id}")
    .addKey(keyCredential,passwordCredential,proof)
    .buildRequest()
    .post();

```