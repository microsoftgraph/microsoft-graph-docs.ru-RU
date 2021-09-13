---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e2e31181b2d35295e2d29e65269998361e46fb64daa250d9208133918cdd95f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtensions = await client.api('/schemaExtensions')
    .filter('id eq \'graphlearn_test\'')
    .get();

```