---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92d7223a8e52cf33bcdebb99421aceca0ab385cf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
    clientSecret: "1111111111111"
};

let res = await client.api('/identityProviders/Amazon-OAuth')
    .update({identityProvider : identityProvider});

```