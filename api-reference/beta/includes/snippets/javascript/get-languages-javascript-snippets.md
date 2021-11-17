---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 689a41ca500d7bda03fa5aea6bf76f00bd2f36e34e297f9c42cf1ad5f4cdd257
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/me/profile/languages')
    .version('beta')
    .get();

```