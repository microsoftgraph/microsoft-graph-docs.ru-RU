---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d9bcf876788bcc5660f66747fcfe176b6dd702f9b8ef4768aa763b27474a9694
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57205046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/identityProviders')
    .version('beta')
    .get();

```