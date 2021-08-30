---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 45df772bef90fa6533293217b922e92693352df8c03f8bdcc845ad67fe9d60f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57212006"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let findRoomLists = await client.api('/me/findRoomLists')
    .version('beta')
    .get();

```