---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 317f4d49f5ee8c532b2fe46d814f91ef4b049b65
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/restart')
    .version('beta')
    .post();

```