---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03883eab832b954c29f412070c15bd927d31c9347a3bc0a318b89244cf59e2d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/contactFolders/{id}/contacts/delta')
    .header('Prefer','odata.maxpagesize=2')
    .select('displayName')
    .get();

```