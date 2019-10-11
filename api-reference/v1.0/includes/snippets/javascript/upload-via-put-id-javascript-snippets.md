---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 022e351463736845597cee77705e75172fbd933f
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "37429225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = The contents of the file goes here.;

let res = await client.api('/me/drive/items/{item-id}/content')
    .put(stream);

```