---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f438b194b3c8ef93a22bab786311cb30c14babeb066458f8b296fc0a05102f45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306303"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlows = await client.api('/identity/userFlows')
    .version('beta')
    .get();

```