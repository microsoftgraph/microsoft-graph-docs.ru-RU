---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 23553a3f715513f5e8e6bbc925163bb54d2c82b7
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a')
    .version('beta')
    .delete();

```