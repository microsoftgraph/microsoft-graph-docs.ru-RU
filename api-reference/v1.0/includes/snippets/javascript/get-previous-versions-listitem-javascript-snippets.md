---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8d6637265d5aff221c17a3f827ce6edab119abd6cd3c1c11e5cc2d754c89f670
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57369318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let versions = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions')
    .get();

```