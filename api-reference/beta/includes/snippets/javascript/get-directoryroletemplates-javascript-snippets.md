---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 11298e45c63eff7d30d33ad0e6613bd242c6dff752af8d577f87aaf70289482c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoleTemplates = await client.api('/directoryRoleTemplates')
    .version('beta')
    .get();

```