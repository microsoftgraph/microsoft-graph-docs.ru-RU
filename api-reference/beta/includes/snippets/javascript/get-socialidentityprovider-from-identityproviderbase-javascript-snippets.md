---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 581c99678f859ef7d5ceaf7df507a5630f43e7d2
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/Amazon-OAUTH')
    .version('beta')
    .get();

```