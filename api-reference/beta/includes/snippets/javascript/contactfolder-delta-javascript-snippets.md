---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 667c4bce56dc0a8a44aa039dbe8e6a39d72e07f1faa9143ffdc033724d4f5bae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/contactFolders/delta')
    .version('beta')
    .get();

```