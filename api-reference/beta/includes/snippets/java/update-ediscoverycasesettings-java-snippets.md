---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 501446614ae9b143853606a8648559398d3a752a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092437"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCaseSettings ediscoveryCaseSettings = new EdiscoveryCaseSettings();
RedundancyDetectionSettings redundancyDetection = new RedundancyDetectionSettings();
ediscoveryCaseSettings.redundancyDetection = redundancyDetection;
TopicModelingSettings topicModeling = new TopicModelingSettings();
ediscoveryCaseSettings.topicModeling = topicModeling;
OcrSettings ocr = new OcrSettings();
ediscoveryCaseSettings.ocr = ocr;

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").settings()
    .buildRequest()
    .patch(ediscoveryCaseSettings);

```