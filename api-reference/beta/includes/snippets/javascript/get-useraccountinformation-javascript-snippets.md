---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c7cf35b2348b47308809e421a7fef9d8594688d564723e6cb4d55046e96643b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57370171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAccountInformation = await client.api('/me/profile/account/{id}')
    .version('beta')
    .get();

```