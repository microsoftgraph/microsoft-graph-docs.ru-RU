---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7afd712f3ef8ba18b0ccd18e47fdd32395d868ff
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000')
    .version('beta')
    .get();

```