---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 026ad721ce8881effb2bdd1439bbe935a74a3ba8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordSingleSignOnCredentialSet = {
  id: '5793aa3b-cca9-4794-679a240f8b58'
};

await client.api('/servicePrincipals/{id}/getPasswordSingleSignOnCredentials')
    .version('beta')
    .post(passwordSingleSignOnCredentialSet);

```