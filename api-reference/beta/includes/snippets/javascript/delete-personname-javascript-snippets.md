---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aede655189ebe41da5b2b5434936331f85743f75cf8bee36e050cc308378a86c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/names/{id}')
    .version('beta')
    .delete();

```