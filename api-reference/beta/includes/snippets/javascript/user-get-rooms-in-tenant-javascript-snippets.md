---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6f42b3d923150b3c52b0a0ed2d47a2a8ff916065112db4f6c1b861c02855ca16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57258053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let findRooms = await client.api('/me/findRooms')
    .version('beta')
    .get();

```