---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f31e0b0df08a302cdb312519eedbd1ce93c34e27
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnniversary = {
  type: "birthday",
  date: "1980-01-08"
};

let res = await client.api('/me/profile/anniversaries')
    .version('beta')
    .post(personAnniversary);

```