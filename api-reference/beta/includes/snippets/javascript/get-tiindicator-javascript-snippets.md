---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: da21c1f2649247f24914723084ce95acd907284f9df4e794f91b0bc867fc69be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tiIndicator = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .get();

```