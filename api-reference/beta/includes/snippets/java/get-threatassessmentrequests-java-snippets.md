---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ddfb26818f89836f9028ac6578efb2ce09e8a9f6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952955"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IThreatAssessmentRequestCollectionPage threatAssessmentRequests = graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .get();

```