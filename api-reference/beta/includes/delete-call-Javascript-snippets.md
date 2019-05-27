---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 52de1a8d89cd21c6b24b3e062c28b3f80903908b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}')
    .version('beta')
    .delete();

```