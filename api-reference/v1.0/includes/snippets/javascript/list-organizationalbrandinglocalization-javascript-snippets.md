---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 66eace78cb5ccb51674afbf896e9fb3990425bb9
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let localizations = await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding/localizations/')
    .get();

```