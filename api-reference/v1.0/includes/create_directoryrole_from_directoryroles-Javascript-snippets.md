---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8afbfcb8ddb7650b27badb4fab6589f9aa8cbefd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  roleTemplateId: "roleTemplateId-value"
};

let res = await client.api('/directoryRoles')
    .post({directoryRole : directoryRole});

```