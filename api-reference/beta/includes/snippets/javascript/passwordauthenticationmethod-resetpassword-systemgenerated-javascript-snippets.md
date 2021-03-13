---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ac0c7b9bf87d4e70c0697d6c783452d631f0637d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword')
    .version('beta')
    .post();

```