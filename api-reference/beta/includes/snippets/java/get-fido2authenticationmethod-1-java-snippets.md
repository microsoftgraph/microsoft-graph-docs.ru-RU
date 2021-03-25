---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5968be2ffaf7b5229a319a6b78e9111de6f114b9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209632"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Fido2AuthenticationMethod fido2AuthenticationMethod = graphClient.me().authentication().fido2Methods("-2_GRUg2-HYz6_1YG4YRAQ2")
    .buildRequest()
    .get();

```