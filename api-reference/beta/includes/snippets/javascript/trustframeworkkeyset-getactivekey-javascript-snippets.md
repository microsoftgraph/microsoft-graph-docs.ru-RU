---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff1b9bea7896a329bf40719d267cd23832598839b8c2612b235675e7235bb9b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57310098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let trustFrameworkKey = await client.api('/trustFramework/keySets/{id}/getActiveKey')
    .version('beta')
    .get();

```