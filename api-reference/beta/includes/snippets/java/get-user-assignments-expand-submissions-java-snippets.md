---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f6659b70242654ac9ad670edfbf71d213dbe912e
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730195"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "submissions"));

EducationAssignmentCollectionPage assignments = graphClient.education().users("80cefd93-8d88-40e2-b5d3-67898383e226").assignments()
    .buildRequest( requestOptions )
    .get();

```