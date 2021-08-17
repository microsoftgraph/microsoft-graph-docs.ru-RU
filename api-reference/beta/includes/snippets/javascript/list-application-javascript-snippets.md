---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96494e228eab8f6dfa6ff78d6a01488846bf2d8cfb325574b75b27763c804f69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57246419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/applications')
    .version('beta')
    .get();

```