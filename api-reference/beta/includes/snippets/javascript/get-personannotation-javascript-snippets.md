---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee95bf117b66affb5980affcd149f02836c6e4188c86b2acc19864c1950aef28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personAnnotation = await client.api('/me/profile/notes/{id}')
    .version('beta')
    .get();

```