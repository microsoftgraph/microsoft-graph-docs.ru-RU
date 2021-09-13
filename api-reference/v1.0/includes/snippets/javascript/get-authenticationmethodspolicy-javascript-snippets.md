---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 83686f7e940f03846e2c6f675837457f2c5df6590f69df047de9935d25189d93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodsPolicy = await client.api('/policies/authenticationMethodsPolicy')
    .get();

```