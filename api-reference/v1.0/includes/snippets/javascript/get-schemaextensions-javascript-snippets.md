---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ebbb537404daf7294b416ea1b67c9234ddbb199f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions')
    .filter('id eq \'graphlearn_test\'')
    .get();

```