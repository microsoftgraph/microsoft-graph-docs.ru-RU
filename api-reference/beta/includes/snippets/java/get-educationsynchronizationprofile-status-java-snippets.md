---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 95dd0640ade32134fd548ebd3c661e79b1e6c97d605c72f33c86e3cf74637644
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57393953"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSynchronizationProfileStatus educationSynchronizationProfileStatus = graphClient.education().synchronizationProfiles("{id}").profileStatus()
    .buildRequest()
    .get();

```