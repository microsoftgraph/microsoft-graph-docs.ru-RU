---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3735de0ba64d32f08697e28449d379c2543b3c20480639b68da1fa1135f92db9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groupSettings/{id}')
    .delete();

```