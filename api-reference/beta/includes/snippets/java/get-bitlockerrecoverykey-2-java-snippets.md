---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 00896ee2f6d145a84bf39c5448525d55e4a73b56
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944375"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ocp-client-name", "\"My Friendly Client\""));
requestOptions.add(new HeaderOption("ocp-client-version", "\"1.2\""));

IBitlockerRecoveryKeyCollectionPage recoveryKeys = graphClient.informationProtection().bitlocker().recoveryKeys()
    .buildRequest( requestOptions )
    .filter("deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'")
    .get();

```