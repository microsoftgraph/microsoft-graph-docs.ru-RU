---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3dbe06ec13dde034ac215d47b405528a03ec76371baec7c9488a929d29b11765
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57395052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let thumbnails = await client.api('/me/drive/items/{item-id}/thumbnails')
    .get();

```