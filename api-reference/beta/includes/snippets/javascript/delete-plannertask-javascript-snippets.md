---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6c8cf72f01ed22763586a7f99420aa934c94b98df859a97450d2320348eec946
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/tasks/{id}')
    .version('beta')
    .delete();

```