---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81bd48514e050739f10a5a1fe8ce1ab82f3f4be78d7ac9e69529ce598b8a6c58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57205099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group')
    .version('beta')
    .get();

```