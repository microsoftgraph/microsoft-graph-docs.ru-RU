---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 144ece94b95d0d32662cbf308ebd0fb9da1f113f0e37baaf58d3f2029c88cae5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .filter('appDefinitions/any(a:a/bot ne null)')
    .expand('appDefinitions($expand=bot)')
    .get();

```