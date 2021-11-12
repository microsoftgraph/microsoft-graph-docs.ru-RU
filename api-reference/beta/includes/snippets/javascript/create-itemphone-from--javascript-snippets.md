---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d27ac902c2dfbb8473778b416ebed64f368898aad3d66afc91c5306dfd395b2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57370330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPhone = {
  displayName: 'Car Phone',
  number: '+7 499 342 22 13'
};

await client.api('/me/profile/phones')
    .version('beta')
    .post(itemPhone);

```