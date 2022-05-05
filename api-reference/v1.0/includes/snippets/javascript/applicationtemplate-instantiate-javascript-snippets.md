---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 873786b555dddc11d1d30752c2786b25c2f2631c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applicationServicePrincipal = {
    displayName: 'Azure AD SAML Toolkit'
};

await client.api('/applicationTemplates/229946b9-a9fb-45b8-9531-efa47453ac9e/instantiate')
    .post(applicationServicePrincipal);

```