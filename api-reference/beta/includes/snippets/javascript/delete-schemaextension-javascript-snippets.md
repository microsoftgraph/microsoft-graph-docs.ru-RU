---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: deb7587f02821e243c34675febb58f877575b2f4125db9b70bf1e9047adf413a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57211970"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/schemaExtensions/{id}')
    .version('beta')
    .delete();

```