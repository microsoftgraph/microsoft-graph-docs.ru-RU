---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7dba90973427232df1b82e8c2eaf17edcbed4a6b8cb3c0ced7a048f239c8a22c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57204207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/tasks('AAMkADA1MT15rfAAA=')/complete')
    .version('beta')
    .post();

```