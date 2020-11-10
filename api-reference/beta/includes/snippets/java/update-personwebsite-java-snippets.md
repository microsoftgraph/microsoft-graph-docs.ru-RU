---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 50dce55ee51f2160abe773a78ec1d4741c7bc1e0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971270"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsite personWebsite = new PersonWebsite();
personWebsite.description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway";

graphClient.me().profile().websites("{id}")
    .buildRequest()
    .patch(personWebsite);

```