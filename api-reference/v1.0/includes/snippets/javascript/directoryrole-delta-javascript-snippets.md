---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 699d450a118bfb5fa4dd09982c92bcb1e4f966f659952256eb312e5dcf169e68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57153195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/directoryRoles/delta')
    .get();

```