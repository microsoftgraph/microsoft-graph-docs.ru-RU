---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 613ecc284c44f4340ada47febedb3e9ff28d4cb8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements/{id}')
    .version('beta')
    .delete();

```