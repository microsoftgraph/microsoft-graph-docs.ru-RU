---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7090bee868a9a679dd2dbdf3cace47713484cd408afe9c27e2db270fddfa245b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57362450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/contactFolders/{id}/contacts/delta')
    .version('beta')
    .select('displayName')
    .get();

```