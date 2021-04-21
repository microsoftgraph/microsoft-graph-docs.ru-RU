---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f711600ac2ccf6bba468fbb2bc228dd7f0aa5773
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920341"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: 'Partner',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1,
    identityProviders: [
        {
            id: 'Facebook-OAuth',
            type: 'Facebook',
            name: 'Facebook'
        }
    ]
};

await client.api('/identity/b2xUserFlows')
    .post(b2xIdentityUserFlow);

```