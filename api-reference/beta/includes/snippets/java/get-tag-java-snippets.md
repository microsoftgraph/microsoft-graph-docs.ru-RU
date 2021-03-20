---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 497e24063b2513adc21ed5bd25f78100bd54afe3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968561"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Tag tag = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("e54b3f535b434a9a8743b84e34c00504")
    .buildRequest()
    .get();

```