---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d39f2bf07edc9191033b1d3afbf6ec5c6db4ab6c381e718ee8f87c34eebf229f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57368570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendars = await client.api('/me/calendars')
    .version('beta')
    .get();

```