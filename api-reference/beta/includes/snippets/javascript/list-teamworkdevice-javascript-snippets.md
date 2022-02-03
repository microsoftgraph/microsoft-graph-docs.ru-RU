---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14e509274b2ef68da2004406155920f2010eab63
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/teamwork/devices')
    .version('beta')
    .get();

```