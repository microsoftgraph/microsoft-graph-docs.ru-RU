---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ea03a47bcd4e4f66d48940a6efbeddfa6376437b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972013"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Tag tag = new Tag();
tag.displayName = "Privileged";
tag.description = "The document is privileged";
tag.additionalDataManager().put("parent@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags()
    .buildRequest()
    .post(tag);

```