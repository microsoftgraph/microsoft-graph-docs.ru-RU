---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3a7287782774aebdb31d5a0ae4c840c407b25791b60c13e8d37442ab90c46ab2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57307920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userCredentialUsageDetails = await client.api('/reports/userCredentialUsageDetails')
    .version('beta')
    .get();

```