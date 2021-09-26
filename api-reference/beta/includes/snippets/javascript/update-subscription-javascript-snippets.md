---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7016562043337eeb3c93e901502efa250971b51004217207a95e5f4109b98330
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57208545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   expirationDateTime: '2016-11-22T18:23:45.9356913Z'
};

await client.api('/subscriptions/{id}')
    .version('beta')
    .update(subscription);

```