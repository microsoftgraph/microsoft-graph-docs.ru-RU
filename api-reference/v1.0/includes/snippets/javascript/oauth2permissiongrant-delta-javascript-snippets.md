---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6e8c2e2d0ede6bba579df95ea21db68888e3b075846deb38161bbb621d913581
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57319397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/oauth2PermissionGrants/delta')
    .get();

```