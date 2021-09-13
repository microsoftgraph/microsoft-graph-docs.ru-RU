---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ed636ed837fe82a29eafb892b36174d1b415f93634ec3646b1a5704cc1db850
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/users/{user-id}')
    .delete();

```