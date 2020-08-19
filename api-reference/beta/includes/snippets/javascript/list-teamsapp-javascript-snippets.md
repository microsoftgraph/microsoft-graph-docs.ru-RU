---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9f50fa9b0f680eb5c93af9f4da72006d76fbd968
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'')
    .get();

```