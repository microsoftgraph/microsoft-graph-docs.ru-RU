---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 02111253d0a505025236bf19b99baef6ea86fe28ee4a48aa6b106b0e625285b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57207411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tags = await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags')
    .version('beta')
    .get();

```