---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6426900bcae37c7932365d20a3016255d7b71e1f
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changeScreenSharingRole = {
  role: "viewer"
};

let res = await client.api('/communications/calls/{id}/changeScreenSharingRole')
    .version('beta')
    .post(changeScreenSharingRole);

```