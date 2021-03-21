---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ab6ff611b215cbdf05d29ab57ed6ad017ce8d265
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordlessMicrosoftAuthenticatorMethods = await client.api('/me/authentication/passwordlessMicrosoftAuthenticatorMethods')
    .version('beta')
    .get();

```