---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b1e8eac45454a2ea3547bb3dbb04edcac1d7ad5a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/Apple-Managed-OIDC')
    .version('beta')
    .get();

```