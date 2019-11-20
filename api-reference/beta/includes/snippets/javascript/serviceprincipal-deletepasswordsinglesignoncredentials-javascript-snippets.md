---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a06255a31fcfea2abd2ee9528485db70a48fd3fb
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const deletePasswordSingleSignOnCredentials = {
  id: "5793aa3b-cca9-4794-679a240f8b58"
};

let res = await client.api('/servicePrincipals/{id}/deletePasswordSingleSignOnCredentials')
    .version('beta')
    .post(deletePasswordSingleSignOnCredentials);

```