---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 857ff74899b2f5f2601edd0639a015153fde8c33
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610701"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrants = await client.api('/chats/19:089ac694c48647c68035aae675cf78ab@thread.v2/permissionGrants')
    .version('beta')
    .get();

```