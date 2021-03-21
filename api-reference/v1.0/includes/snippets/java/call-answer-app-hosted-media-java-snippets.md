---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c04ca7be4b6562ebfd3ca56cf2ff285172743286
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975747"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String callbackUri = "https://bot.contoso.com/api/calls";

LinkedList<Modality> acceptedModalitiesList = new LinkedList<Modality>();
acceptedModalitiesList.add(Modality.AUDIO);

AppHostedMediaConfig mediaConfig = new AppHostedMediaConfig();
mediaConfig.blob = "<Media Session Configuration Blob>";

graphClient.communications().calls("57DAB8B1894C409AB240BD8BEAE78896")
    .answer(CallAnswerParameterSet
        .newBuilder()
        .withCallbackUri(callbackUri)
        .withMediaConfig(mediaConfig)
        .withAcceptedModalities(acceptedModalitiesList)
        .build())
    .buildRequest()
    .post();

```