---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6e027cf5f07768786f29ddd24acf173fb260bbe5371eea0ad50d724f405fae1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57199513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: '65415bb1-9267-4313-bbf5-ae259732ee12'
};

await client.api('/servicePrincipals')
    .post(servicePrincipal);

```