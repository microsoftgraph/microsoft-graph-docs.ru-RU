---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e1e9b133f7dc0a65ff54c5717765a3360d1ab59988439966b85df4e6f032dc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57268465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recent = await client.api('/me/activities/recent')
    .get();

```