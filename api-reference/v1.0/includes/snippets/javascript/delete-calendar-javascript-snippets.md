---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 76f2b1f3331ba43d87d11fe5c2fb7b372b96a82d2a4de50b74bbaedf4e2d8b82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendar')
    .delete();

```