---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7213f87399eccab25ade4c43ef8f2353bb6d5ab55cdb51cad26863b7501c9743
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .version('beta')
    .header('Prefer','return=minimal')
    .select('displayName,description,mailNickname')
    .get();

```