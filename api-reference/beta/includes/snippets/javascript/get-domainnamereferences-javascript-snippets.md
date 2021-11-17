---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c74b6a56358cf275734b3b58d374401e43e4e646916eedd1fee90896a089f9db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57250237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domainNameReferences = await client.api('/domains/contoso.com/domainNameReferences')
    .version('beta')
    .get();

```