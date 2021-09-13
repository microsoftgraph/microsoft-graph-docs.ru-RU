---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0bd91c7741e4e69565e0a4b080e02140c6e1ef5a9709275be581b20ddfa3d115
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57374189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = The contents of the file goes here.;

await client.api('/me/drive/items/{item-id}/content')
    .put(stream);

```