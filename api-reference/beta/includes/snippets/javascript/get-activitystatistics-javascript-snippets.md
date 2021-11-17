---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b30166e507e5d9d1dfb431617f5e4d1ab00af10674117aa610f24dc2125370d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050942"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityStatistics = await client.api('/me/analytics/activitystatistics')
    .version('beta')
    .get();

```