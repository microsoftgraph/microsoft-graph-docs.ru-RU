---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b33bb0f84642bb978d63bfdea09cf8f5ed857204b663f86726200713bbe11af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57253775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/completeMigration')
    .post();

```