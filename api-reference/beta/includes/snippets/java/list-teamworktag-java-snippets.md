---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14f730212d94cfbc366387beb17580df2296e6f783aa6ebb7b8c62c1fd1112ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57251759"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkTagCollectionPage tags = graphClient.teams("53c53217-fe77-4383-bc5a-ed4937a1aecd").tags()
    .buildRequest()
    .get();

```